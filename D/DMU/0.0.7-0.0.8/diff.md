# Comparing `tmp/DMU-0.0.7.tar.gz` & `tmp/DMU-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DMU-0.0.7.tar", last modified: Thu Jun 29 11:53:10 2023, max compression
+gzip compressed data, was "DMU-0.0.8.tar", last modified: Thu Jul  6 10:50:26 2023, max compression
```

## Comparing `DMU-0.0.7.tar` & `DMU-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 11:53:10.745525 DMU-0.0.7/
-drwxrwxrwx   0        0        0        0 2023-06-29 11:53:10.745525 DMU-0.0.7/DMU/
--rw-rw-rw-   0        0        0        0 2023-06-29 11:52:30.000000 DMU-0.0.7/DMU/__init__.py
--rw-rw-rw-   0        0        0      713 2023-06-29 11:52:30.000000 DMU-0.0.7/DMU/graph_styles.py
--rw-rw-rw-   0        0        0   114227 2023-06-29 11:52:30.000000 DMU-0.0.7/DMU/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-29 11:53:10.745525 DMU-0.0.7/DMU.egg-info/
--rw-rw-rw-   0        0        0    11119 2023-06-29 11:53:10.000000 DMU-0.0.7/DMU.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2023-06-29 11:53:10.000000 DMU-0.0.7/DMU.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 11:53:10.000000 DMU-0.0.7/DMU.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-06-29 11:53:10.000000 DMU-0.0.7/DMU.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-29 11:53:10.000000 DMU-0.0.7/DMU.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1102 2023-06-29 11:52:30.000000 DMU-0.0.7/LICENSE
--rw-rw-rw-   0        0        0    11119 2023-06-29 11:53:10.745525 DMU-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0    10503 2023-06-29 11:52:30.000000 DMU-0.0.7/README.md
--rw-rw-rw-   0        0        0       42 2023-06-29 11:53:10.745525 DMU-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     3608 2023-06-29 11:52:30.000000 DMU-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 10:50:26.391166 DMU-0.0.8/
+drwxrwxrwx   0        0        0        0 2023-07-06 10:50:26.391166 DMU-0.0.8/DMU/
+-rw-rw-rw-   0        0        0        0 2023-07-06 10:49:46.000000 DMU-0.0.8/DMU/__init__.py
+-rw-rw-rw-   0        0        0      713 2023-07-06 10:49:46.000000 DMU-0.0.8/DMU/graph_styles.py
+-rw-rw-rw-   0        0        0   110025 2023-07-06 10:49:46.000000 DMU-0.0.8/DMU/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-06 10:50:26.391166 DMU-0.0.8/DMU.egg-info/
+-rw-rw-rw-   0        0        0    11119 2023-07-06 10:50:26.000000 DMU-0.0.8/DMU.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2023-07-06 10:50:26.000000 DMU-0.0.8/DMU.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 10:50:26.000000 DMU-0.0.8/DMU.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-07-06 10:50:26.000000 DMU-0.0.8/DMU.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-06 10:50:26.000000 DMU-0.0.8/DMU.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1102 2023-07-06 10:49:46.000000 DMU-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0    11119 2023-07-06 10:50:26.391166 DMU-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0    10503 2023-07-06 10:49:46.000000 DMU-0.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-06 10:50:26.391166 DMU-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     3608 2023-07-06 10:49:46.000000 DMU-0.0.8/setup.py
```

### Comparing `DMU-0.0.7/DMU/graph_styles.py` & `DMU-0.0.8/DMU/graph_styles.py`

 * *Files identical despite different names*

### Comparing `DMU-0.0.7/DMU/utils.py` & `DMU-0.0.8/DMU/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,90 +51,90 @@
         P_tot.append(np.sum(BivarSpline))
     
     return(P_tot)
 
 #%%
 
 def bias_plotter(data,FIG,**kwargs): 
-    
+    ax = FIG.ax[0]
     IFIG = False
     IDF = None
     keys = list(data.keys())
     kwargdict = {'fwd':'fwd','f':'fwd','forward':'fwd',
                  'bwd':'rev','rev':'rev','reverse':'rev',
                  'title':'title','tit':'title',
                  'tool':'tool','experiment':'exp','exp':'exp',
-                 'ideality':'ideality',
-                 'plot':'plot'}
+                 'ideality':'ideality'}
     
     kuniq = np.unique(list(kwargdict.keys()))
     Pkwargs = {}
     #Filtering out the function kwargs from the plot kwargs
     for key in kwargs.keys():
         if key not in kuniq:
             kwargdict[key] = key
     #Collecting kwargs
-    kw = KwargEval(kwargs, kwargdict,fwd = True, rev = True, title=None,tool="Nanonis",exp='2IV',ideality=False,plot=True)
+    kw = KwargEval(kwargs, kwargdict,fwd = True, rev = True, title=None,tool="Nanonis",exp='2IV',ideality=False)
     xkey = []; ykey = []; fwdbwd = []
-    if kw.plot == True:
-        ax = FIG.ax[0]
-        
+    
     #Separating plot kwargs into a different dict
     for key,val in kwargs.items():
         if key not in kuniq:
             Pkwargs[key] = val
             
     
     if kw.tool == "Nanonis":
-        if kw.plot == True:
-            for k in keys:
-                if "bias" in k.lower():
-                    xkey.append(k)
-                    
-                if "bwd" not in k.lower() and "bias" not in k.lower():
-                    ykey.append(k)
-                    fwdbwd.append(0) #Note: 0  is forward, 1 is backwards
-                
-                if "bwd" in k.lower() and "bias" not in k.lower():
-                    ykey.append(k)
-                    fwdbwd.append(1) #Note: 0  is forward, 1 is backwards
-            
-            for n,i in enumerate(fwdbwd):    
-                plotkwargs = {}
-                for k,v in Pkwargs.items():
-                    try: 
-                        plotkwargs[k] = v[i]
-                    except:
-                        plotkwargs[k] = v
+        for k in keys:
+            if "bias" in k.lower():
+                xkey.append(k)
+                
+            if "bwd" not in k.lower() and "bias" not in k.lower():
+                ykey.append(k)
+                fwdbwd.append(0) #Note: 0  is forward, 1 is backwards
             
-                if kw.fwd == True and i == 0:
-                    ax.plot(data[xkey[0]],data[ykey[i]],label='Forward',**plotkwargs)
-                    
-                if kw.rev == True and i == 1:
-                    ax.plot(data[xkey[0]],data[ykey[i]],label='Backward',**plotkwargs)
+            if "bwd" in k.lower() and "bias" not in k.lower():
+                ykey.append(k)
+                fwdbwd.append(1) #Note: 0  is forward, 1 is backwards
+        
+        for n,i in enumerate(fwdbwd):    
+            plotkwargs = {}
+            for k,v in Pkwargs.items():
+                try: 
+                    plotkwargs[k] = v[i]
+                except:
+                    plotkwargs[k] = v
+        
+            if kw.fwd == True and i == 0:
+                ax.plot(data[xkey[0]],data[ykey[i]],label='Forward',**plotkwargs)
                 
-            ax.set_xlabel(xkey[0])
-            ax.set_ylabel(ykey[fwdbwd[0]])
-            ax.legend()
-            ax.set_title(kw.title)
+            if kw.rev == True and i == 1:
+                ax.plot(data[xkey[0]],data[ykey[i]],label='Backward',**plotkwargs)
+            
+        ax.set_xlabel(xkey[0])
+        ax.set_ylabel(ykey[fwdbwd[0]])
+        ax.legend()
+        ax.set_title(kw.title)
         
         if kw.ideality == True:
-        
-            tab20 = mcm.get_cmap("tab20",20)
-            IFIG = True
-            IDF = Ideality_Factor(data[ykey[0]],data[xkey[0]])
-            if kw.plot == True:
+            
+            #try:
+                tab20 = mcm.get_cmap("tab20",20)
+                IFIG = True
+                print(len(data[ykey[0]]))
+                print(len(data[xkey[0]]))
+                IDF = Ideality_Factor(data[ykey[0]],data[xkey[0]],273,[1.3,2],[1.3,2],100,[1e-8, 3])
+                
                 IFIG = ezplot()
-    
+
                 IFIG.ax[0].plot(IDF['V_new'],IDF['I_new'],'.-',linewidth=2,color=tab20(0),label='ideality='+"{0:.5g}".format(IDF['n']))
                 IFIG.ax[0].plot(IDF['V'],IDF['I'],'.',linewidth=2,c=tab20(1),label='IV data')
-    
-    
+
+
                 IFIG.ax[0].legend()
-            
+            #except:
+                None
                 
     elif kw.tool == "Keithley":
         keys = data['col headers']
         plotkwargs = {}
         
         for i,ll in enumerate(xkey):
             for k,v in Pkwargs.items():
@@ -146,105 +146,103 @@
         for k in keys:
             if "voltage" in k.lower():
                 xkey.append(k)
             elif "current" in k.lower():
                 ykey.append(k)
         
         xkey.sort(); ykey.sort()
-        if kw.plot == True:
-            if "Voltage Linear Sweep" in data["Settings"]["Operation Mode"]:
-                if len(xkey) == 1 and len(ykey) == 1:
+        
+        if "Voltage Linear Sweep" in data["Settings"]["Operation Mode"]:
+            if len(xkey) == 1 and len(ykey) == 1:
+                for m,data_x in enumerate(data[xkey[0]]): 
+                    ax.plot(data[xkey[0]][m],data[ykey[0]][m],label=ykey[0],**plotkwargs)
+            
+            elif len(xkey) > 1 and len(ykey)>1:
+                for n,key in enumerate(xkey):
                     for m,data_x in enumerate(data[xkey[0]]): 
-                        ax.plot(data[xkey[0]][m],data[ykey[0]][m],label=ykey[0],**plotkwargs)
-                
-                elif len(xkey) > 1 and len(ykey)>1:
-                    for n,key in enumerate(xkey):
-                        for m,data_x in enumerate(data[xkey[0]]): 
-                            ax.plot(data[xkey[n]][m],data[ykey[n]][m],label=ykey[n],**plotkwargs)
-                        
-                elif len(xkey) == 1 and len(ykey)>1:
-                    for n,key in enumerate(ykey):
-                        for m,data_x in enumerate(data[xkey[0]]):
-                            ax.plot(data[xkey[0]][m],data[ykey[n]][m],label=ykey[n],**plotkwargs)
-                        
-                elif len(xkey) > 1 and len(ykey)==1:
-                    for n,key in enumerate(xkey):
-                        for m,data_x in enumerate(data[xkey[0]]):
-                            ax.plot(data[xkey[n]][m],data[ykey[0]][m],label=ykey[0],**plotkwargs) 
-                
+                        ax.plot(data[xkey[n]][m],data[ykey[n]][m],label=ykey[n],**plotkwargs)
                     
-                    
-                ax.set_xlabel(xkey[0])
-                ax.set_ylabel(ykey[0])
-                ax.legend()
-                ax.set_title(kw.title)
+            elif len(xkey) == 1 and len(ykey)>1:
+                for n,key in enumerate(ykey):
+                    for m,data_x in enumerate(data[xkey[0]]):
+                        ax.plot(data[xkey[0]][m],data[ykey[n]][m],label=ykey[n],**plotkwargs)
+                    
+            elif len(xkey) > 1 and len(ykey)==1:
+                for n,key in enumerate(xkey):
+                    for m,data_x in enumerate(data[xkey[0]]):
+                        ax.plot(data[xkey[n]][m],data[ykey[0]][m],label=ykey[0],**plotkwargs) 
             
-        if kw.ideality == True:
-            IFIG = False
-            try:
                 
-                tab20 = mcm.get_cmap("tab20",20)
                 
-                IDF = Ideality_Factor(data[ykey[0]][0],data[xkey[0]][0],T=273,plot_range =None,fit_range = None,N=100,p0=None)
-                if kw.plot == True:
+            ax.set_xlabel(xkey[0])
+            ax.set_ylabel(ykey[0])
+            ax.legend()
+            ax.set_title(kw.title)
+            
+            if kw.ideality == True:
+                IFIG = False
+                try:
+                    tab20 = mcm.get_cmap("tab20",20)
+                    
+                    IDF = Ideality_Factor(data[ykey[0]][0],data[xkey[0]][0],273,[1.3,2],[1.3,2],100,[1e-8, 3])
+                    
                     IFIG = ezplot()
     
-                    IFIG.ax[0].plot(IDF['V_new'],IDF['I_new'],'.-',linewidth=1,color=tab20(0),label='ideality='+"{0:.5g}".format(IDF['n']))
+                    IFIG.ax[0].plot(IDF['V_new'],IDF['I_new'],'.-',linewidth=2,color=tab20(0),label='ideality='+"{0:.5g}".format(IDF['n']))
                     IFIG.ax[0].plot(IDF['V'],IDF['I'],'.',linewidth=2,c=tab20(1),label='IV data')
     
     
                     IFIG.ax[0].legend()
-                
-            except:
-                None
+                    
+                except:
+                    None
                     
         elif "Voltage List Sweep" in data["Settings"]["Operation Mode"]:
-            if kw.plot == True:
-                FIG.fig,(FIG.ax[0],FIG.ax[1]) = plt.subplots(nrows=2, sharex=True)
-                fig, ax_top, ax_bottom = [FIG.fig,FIG.ax[0],FIG.ax[1]]
-                ax_top.spines["bottom"].set_visible(False)
-                ax_bottom.spines["top"].set_visible(False)
-                ax_top.tick_params(bottom=False)
-                ax_bottom.tick_params(top=False)
-                plt.subplots_adjust(hspace=0.1)
-        
-                ax_top_r = ax_top.twinx()
-                ax_bottom_r = ax_bottom.twinx()
-                
-                axyy  = [ax_top,ax_bottom]
-                axxy  = [ax_top_r,ax_bottom_r]
-                if len(xkey) == 1 and len(ykey)>1:
-                    for n,key in enumerate(ykey):
-                        axyy[n].plot(data[ykey[n]][0],label=ykey[n],**plotkwargs)
-                        axxy[n].plot(data[xkey[0]][0],label=xkey[0],**plotkwargs)
-                        axyy[n].set_ylabel(ykey[n][0])
-                        axxy[n].set_ylabel(xkey[0][0])
-                        
-                if len(xkey) > 1 and len(ykey)>1:
-                    for n,key in enumerate(ykey):
-                        axyy[n].plot(data[ykey[n]][0],label=ykey[n],**plotkwargs)
-                        axxy[n].plot(data[xkey[1]][0],label=xkey[1],**plotkwargs)
-                        axyy[n].set_ylabel(ykey[n][0] + " [A]",color='blue')
-                        axxy[n].set_ylabel(xkey[1][0] + " [V]",color='orange')
-                    #Fix colours
-                if len(Pkwargs['c'])<4:
-                    Pkwargs['c'] = mcm.get_cmap("tab20",20)
-                for axis in axyy:
-                    for i,line in enumerate(axis.get_lines()):
-                        line.set_color(Pkwargs['c'](i))
-                for axis in axxy:
-                    for i,line in enumerate(axis.get_lines()):
-                        line.set_color(Pkwargs['c'](i+3))
-                ax_bottom.set_xlabel("index")
-                ax_top.set_xlabel("index")
-                handles1,labels = ax_top.get_legend_handles_labels()
-                handles2,labels = ax_top_r.get_legend_handles_labels()
-                fig.legend(handles=handles1+handles2,labels=['$I_{NW}$','$V_{NW}$'])
-     
-                FIG.ax[0].set_title(kw.title)
+            FIG.fig,(FIG.ax[0],FIG.ax[1]) = plt.subplots(nrows=2, sharex=True)
+            fig, ax_top, ax_bottom = [FIG.fig,FIG.ax[0],FIG.ax[1]]
+            ax_top.spines["bottom"].set_visible(False)
+            ax_bottom.spines["top"].set_visible(False)
+            ax_top.tick_params(bottom=False)
+            ax_bottom.tick_params(top=False)
+            plt.subplots_adjust(hspace=0.1)
+    
+            ax_top_r = ax_top.twinx()
+            ax_bottom_r = ax_bottom.twinx()
+            
+            axyy  = [ax_top,ax_bottom]
+            axxy  = [ax_top_r,ax_bottom_r]
+            if len(xkey) == 1 and len(ykey)>1:
+                for n,key in enumerate(ykey):
+                    axyy[n].plot(data[ykey[n]][0],label=ykey[n],**plotkwargs)
+                    axxy[n].plot(data[xkey[0]][0],label=xkey[0],**plotkwargs)
+                    axyy[n].set_ylabel(ykey[n][0])
+                    axxy[n].set_ylabel(xkey[0][0])
+                    
+            if len(xkey) > 1 and len(ykey)>1:
+                for n,key in enumerate(ykey):
+                    axyy[n].plot(data[ykey[n]][0],label=ykey[n],**plotkwargs)
+                    axxy[n].plot(data[xkey[1]][0],label=xkey[1],**plotkwargs)
+                    axyy[n].set_ylabel(ykey[n][0] + " [A]",color='blue')
+                    axxy[n].set_ylabel(xkey[1][0] + " [V]",color='orange')
+                #Fix colours
+            if len(Pkwargs['c'])<4:
+                Pkwargs['c'] = mcm.get_cmap("tab20",20)
+            for axis in axyy:
+                for i,line in enumerate(axis.get_lines()):
+                    line.set_color(Pkwargs['c'](i))
+            for axis in axxy:
+                for i,line in enumerate(axis.get_lines()):
+                    line.set_color(Pkwargs['c'](i+3))
+            ax_bottom.set_xlabel("index")
+            ax_top.set_xlabel("index")
+            handles1,labels = ax_top.get_legend_handles_labels()
+            handles2,labels = ax_top_r.get_legend_handles_labels()
+            fig.legend(handles=handles1+handles2,labels=['$I_{NW}$','$V_{NW}$'])
+ 
+            FIG.ax[0].set_title(kw.title)
             
             
         return(IFIG,IDF)
 
 #%%
 def Single_NW_Diagram_Plotter(fig,ax,NanonisDat):
     """
@@ -1640,32 +1638,23 @@
         pass
     
     #This part initialises the "default" values inside of kwclass using **kwargs. If you don't need any defaults, then you can ignore this.
     if len(kwargs)>0:
         for kwarg in kwargs:
             kval = kwargs.get(kwarg,False)
             try:
-                setattr(kwclass,kwarg, kval)
+                setattr(kwclass,kwargdict[kwarg.lower()], kval)
                 
             except:
                 cprint(['kwarg =',kwarg,'does not exist!',' Skipping kwarg eval.'],mt = ['wrn','err','wrn','note'],co=kwclass.co)
     #Setting the class kwargs from the function kwargs!     
     for kwarg in fkwargs:
-        fkwarg_key = kwarg
-        if kwarg not in kwargdict.keys():
-            kwarg_low = [key.lower() for key in kwargdict.keys()]
-            if kwarg in kwarg_low:
-                kidx = kwarg_low.index(kwarg)
-                kwarg = list(kwargdict.keys())[kidx]
-                
-        kval = kwargs.get(kwarg,False)
-        fkval = fkwargs.get(fkwarg_key,False)
-        
+        fkval = fkwargs.get(kwarg,False)
         try:
-            setattr(kwclass,kwargdict[kwarg], fkval)
+            setattr(kwclass,kwargdict[kwarg.lower()], fkval)
             
         except:
             cprint(['kwarg =',kwarg,'does not exist!',' Skipping kwarg eval.'],mt = ['wrn','err','wrn','note'])
     return(kwclass)
 
 #%%
 def LDI_Data_Import(FLTuple,**kwargs):
@@ -2168,50 +2157,44 @@
         if data[i] <= data[i - 1] or data[i] >= data[i + 1]:
             return True
 
     return False
 
 #%%Finds all indices where the data set changes direction
 def find_turning_points(data):
-    
     turning_points = [0]
-    try:
-        if data[1] > data[0]:
-            increasing = True
-        else:
-            increasing = False
-        step_size = abs(data[int(len(data)/4-2)] - data[int(len(data)/4-3)])
-        sep_tp = []
-        tp_i = 1
-        for i in range(1, len(data)-1):
-            dx = abs(data[i+1] - data[i])
-            if data[i] > data[i+1] and dx > 0.5*step_size:
-                if increasing == True:
-                    turning_points.append(i)
-                    sep_tp.append(turning_points[tp_i] - turning_points[tp_i-1])
-                    tp_i += 1
-                    increasing = False
-                    
-            elif data[i] < data[i+1] and dx > 0.1*step_size:
-                if increasing == False:
-                    turning_points.append(i)
-                    sep_tp.append(turning_points[tp_i] - turning_points[tp_i-1])
-                    tp_i += 1
-                    increasing = True
-                    
-        if len(turning_points) == 1:
-            turning_points = [0,len(data)]
-        elif len(turning_points)>1:
-            turning_points.append(len(data))
-            
-        if max(sep_tp) - min(sep_tp)>3:
-            turning_points = [0,len(data)]
-        return turning_points
-    except:
-        return turning_points
+    if data[1] > data[0]:
+        increasing = True
+    else:
+        increasing = False
+    sep_tp = []
+    tp_i = 1
+    for i in range(1, len(data)-1):
+        if data[i] > data[i+1]:
+            if increasing == True:
+                turning_points.append(i)
+                sep_tp.append(turning_points[tp_i] - turning_points[tp_i-1])
+                tp_i += 1
+                increasing = False
+                
+        elif data[i] < data[i+1]:
+            if increasing == False:
+                turning_points.append(i)
+                sep_tp.append(turning_points[tp_i] - turning_points[tp_i-1])
+                tp_i += 1
+                increasing = True
+                
+    if len(turning_points) == 1:
+        turning_points = [0,len(data)]
+    elif len(turning_points)>1:
+        turning_points.append(len(data))
+        
+    if max(sep_tp) - min(sep_tp)>3:
+        turning_points = [0,len(data)]
+    return turning_points
 
 
 
 #%%Takes a list of lists, then returns them split up where the dependent variable changes direction. 
 
 def segment_sweep(L,indices):
     swdat = []
@@ -2261,50 +2244,41 @@
             keys = [str(cell_value) for cell_value in sheet.row_values(0) if cell_value != ""]
             
             # Convert data to a dictionary with the values in the first row as the keys
             flat_data = {}
             #Determine the SMU position data and create a key for this in flat_data
             smu_ind = [i for i, item in enumerate(keys) if "SMU" in item]
             flat_data['positions'] = {}
-            
             for ind in smu_ind:
                 flat_data['positions']["pos"+str(1+ind - min(smu_ind))] = {}
                 flat_data['positions']["pos"+str(1+ind - min(smu_ind))]['SMU'] = keys[ind]
+            position_indices = [i for i, header in enumerate(keys) if 'POSITION' in header]
             
-            
-            #position_indices = [i for i, header in enumerate(keys) if 'POSITION' in header]
             #This section finds rows that are empty, and excludes them from our search
             for row in rows:
                 if all(x == '' for x in row) != True:
                     if row[0] == "":
-                        if any(string in element for element in row for string in ["NW"]) == True:
-                            for i,var in enumerate(smu_ind):
-    #                            print("smu_ind " + str(var) + " --> produces for -1 = " + str(row[var-1]) +" for 0" + str(row[var]) + " for +1" + str(row[var+1]) )
-                                if row[var] == "":
-                                    flat_data['positions']["pos"+str(1+var-min(smu_ind))]['NW'] = row[var-1]
-                                elif "NW" in row[var]:
-                                    flat_data['positions']["pos"+str(1+var-min(smu_ind))]['NW'] = row[var]
-                            break
-            for row in rows:
-                if all(x == '' for x in row) != True:
-         
+                        for i,var in enumerate(smu_ind):
+                            if row[var] == "":
+                                flat_data['positions']["pos"+str(1+var-min(smu_ind))]['NW'] = row[var-1]
+                            else:
+                                flat_data['positions']["pos"+str(1+var-min(smu_ind))]['NW'] = row[var]
+                        
                     #This section restructures "position" and "nw" to fit with the format desired.    
-                    if row[0] !="":
+                    elif row[0] !="": 
                         run_key = str(int(row[0]))
                         row_dict = {}
                         for i, header in enumerate(keys):
-                            if i in smu_ind:
-                                pos_idx = 1+i-min(smu_ind)
-                                nw_key = 'pos' + str(pos_idx)
-                                row_dict[nw_key] = {'SMU': flat_data['positions']['pos' + str(pos_idx)]['SMU'], 'NW': flat_data['positions']['pos' + str(pos_idx)]['NW']}
-                                    
-                            row_dict[header] = row[i]
-                                
+                            if i in position_indices:
+                                for j, nw_value in enumerate(row[i:i+2]):
+                                    nw_key = 'position ' + str(j+1)
+                                    row_dict[nw_key] = {'SMU': header, 'NW': nw_value}
+                            elif i > 0:
+                                row_dict[header] = row[i]
                         flat_data[run_key] = row_dict
-                        
             file_data = flat_data
             
         data[filename] = file_data
         
         
         
     data_files = [file for file in files if "LOG" not in file ]    
@@ -2377,51 +2351,38 @@
                    
                     if (key.endswith("V") == True and any(s.lower() in key.lower() for s in ["START","STOP"])==False):
                         cols['voltage'] = col_data
                         key = 'voltage'
                     elif (key.endswith("I") == True and any(s.lower() in key.lower() for s in ["START","STOP"])==False):
                         cols['current'] = col_data
                         key = 'current'
-                    if "SD" in key and "voltage" in key:
-                        cols['voltage'] = col_data
-                        key = 'voltage'
-                    if "SD" in key and "current" in key:
-                        cols['current'] = col_data
-                        key = 'current'
-                        
                             
                     cols["col headers"].append(key)
                     
                 #Swap linear sweep data to segmented data 
                 voltage_keys = [key for key in list(cols.keys()) if "voltage" in key.lower()]
 
                 sweep_index_list = []
                 for key in voltage_keys:
                     sweep_index_list.append(find_turning_points(cols[key]))
-                    
                 idx_short = min(range(len(sweep_index_list)), key=lambda i: len(sweep_index_list[i]))
                 sweep_indices = sweep_index_list[idx_short]
                 sweep_length = len(sweep_indices)
                 
                 
                 if len(sweep_indices) < 6 and sweep_indices[0] !=None:
                     sweep_length = len(cols[key])
                         
                 else:
                     sweep_length = None
                             
                 list_keys = [key for key, value in cols.items() if isinstance(value, list)]
                 for key in list_keys:
                     if len(cols[key]) == sweep_length and sweep_length != None:
-                        cols[key]  = segment_sweep(cols[key],sweep_indices)
-                    
-                    else:
-                        if "voltage" == key or "current" == key:
-                            cols[key] = [cols[key]]
-                            
+                        cols[key]  = segment_sweep(cols[key],sweep_indices) 
                 # Store the data in the dictionary
 
                 file_data[sheet_name] = cols
         # Store the data for the file in the top-level dictionary
         data[filename] = file_data
 
         
@@ -2627,97 +2588,34 @@
                 skdict = np.array(skdict)
             out_dict[key] = skdict 
                  
                     
                     
     return(out_dict)
 
-def Ideality_Factor(I,V,**kwargs):
-    kwargdict = {'T':'T','temp':'T','temperature':'T',
-                  'fit_range':'fit_range','fr':'fit_range',
-                  'plot_range':'plot_range','pr':'plot_range',
-                  "data_range":"data_range","dr":"data_range",
-                  'N':'N','pts':'N',
-                  "p0":"p0",'guess':"p0"}
-    
-    kw = KwargEval(kwargs, kwargdict,T=273,fit_range=None,plot_range=None,N=200,p0=None,data_range=None)
-    
+def Ideality_Factor(I,V,T,fit_range,plot_range,N,p0):
     q = constants.e
     k = constants.Boltzmann
     
     def Diode_EQ(V,I_0,n):
-        return(I_0 * np.exp((q*V)/(n*k*kw.T)))    
+        return(I_0 * np.exp((q*V)/(n*k*T)))
     
-
     if max(I) < np.abs(min(I)):
+        I.reverse()
         I = list(np.multiply(-1,I))
-        V = list(np.multiply(-1,V))
-
-    if V[-1]<V[0]:
-        V = np.flip(V)
-        I = np.flip(I)
 
     
-    """
-    if I[0]>I[-1]:
-        V = np.multiply(-1,V)
-        I = np.flip(I)
-    
-    if V[1]-V[0]<0:
-        V = np.flip(V)
-        I = np.flip(I)
-     """   
-        
-    if kw.fit_range == None:
-        kw.fit_range = 0.01
-    
-    
-    if type(kw.fit_range) == float:
-        I_range = [kw.fit_range*max(I),max(I)]
-        
-        v_i =  next((i for i, x in enumerate(I) if x > I_range[0]), -1)
-        v_f =  next((i for i, x in enumerate(I) if x > I_range[1]), -1)
-        kw.fit_range = [V[v_i],V[v_f]]
-        
+    v_i =  next((i for i, x in enumerate(V) if x > fit_range[0]), -1)
+    v_f =  next((i for i, x in enumerate(V) if x > fit_range[1]), -1)
 
     
-    elif type(kw.fit_range) == list:        
-        v_i =  next((i for i, x in enumerate(V) if x > kw.fit_range[0]), -1)
-        v_f =  next((i for i, x in enumerate(V) if x > kw.fit_range[1]), -1)
-     
     V_fit = V[v_i:v_f]
-    I_fit = I[v_i:v_f]
-     
-    if kw.plot_range == "all":
-        kw.plot_range = [min(V),max(V)]
-    
-    elif kw.plot_range == "positive":
-        kw.plot_range = [0,max(V)]
-        
-    elif kw.plot_range == None:
-        kw.plot_range = [min(V_fit),max(V_fit)]
-        
-    if type(kw.data_range) == list:
-        v_id =  next((i for i, x in enumerate(V) if x > kw.data_range[0]), -1)
-        v_fd =  next((i for i, x in enumerate(V) if x > kw.data_range[1]), -1)
-        
-    if kw.data_range == "positive":
-        v_id =  next((i for i, x in enumerate(V) if x > 0), -1)
-        v_fd =  next((i for i, x in enumerate(V) if x > max(V)), -1)
-     
-        V_data = V[v_id:v_fd]
-        I_data = I[v_id:v_fd]
-    else:
-        V_data = V
-        I_data = I
-    
-    if kw.p0 == None:
-        kw.p0 = [kw.fit_range[0]*max(np.abs(I)),3] 
     
+    I_fit = I[v_i:v_f]
 
-    popt, pcov = scipy.optimize.curve_fit(Diode_EQ, V_fit, I_fit,p0=kw.p0)
-    V_new  = np.linspace(kw.plot_range[0],kw.plot_range[1],kw.N)
-    I_new  = Diode_EQ(V_new, *popt)
-
+    popt, pcov = scipy.optimize.curve_fit(Diode_EQ, V_fit, I_fit,p0=p0)
+    V_new = np.linspace(plot_range[0],plot_range[1],N)
+    I_new = Diode_EQ(V_new, *popt)
+    
 
-    return({"n":popt[1],"V_new":V_new,"I_new":I_new,"V_fit":V_fit,"I_fit":I_fit,'V':V,'I':I,'V_data':V_data,"I_data":I_data})
+    return({"n":popt[1],"V_new":V_new,"I_new":I_new,"V":V_fit,"I":I_fit})
```

### Comparing `DMU-0.0.7/DMU.egg-info/PKG-INFO` & `DMU-0.0.8/DMU.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DMU
-Version: 0.0.7
+Version: 0.0.8
 Summary: This package is used to store commonly used functions on pip for the sake of easy pulling for other code.
 Home-page: https://github.com/DeltaMod/DMU
 Author: Atli Vidar Már FLodgren
 Author-email: vidar.flodgren@sljus.lu.se
 Keywords: hello world example examples
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `DMU-0.0.7/LICENSE` & `DMU-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `DMU-0.0.7/PKG-INFO` & `DMU-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DMU
-Version: 0.0.7
+Version: 0.0.8
 Summary: This package is used to store commonly used functions on pip for the sake of easy pulling for other code.
 Home-page: https://github.com/DeltaMod/DMU
 Author: Atli Vidar Már FLodgren
 Author-email: vidar.flodgren@sljus.lu.se
 Keywords: hello world example examples
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `DMU-0.0.7/README.md` & `DMU-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `DMU-0.0.7/setup.py` & `DMU-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 
 setup(
     name="DMU",
-    version="0.0.7",
+    version="0.0.8",
     packages=find_packages(),
     scripts=[TrgtScr],
 
     # Project uses reStructuredText, so ensure that the docutils get
     # installed or upgraded on the target machine
     install_requires=[module_filter(modules)+["docutils>=0.3"]],
```

