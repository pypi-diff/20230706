# Comparing `tmp/morley-0.0.4.tar.gz` & `tmp/morley-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morley-0.0.4.tar", last modified: Thu Mar 16 13:47:16 2023, max compression
+gzip compressed data, was "morley-0.0.5.tar", last modified: Thu Jul  6 14:16:21 2023, max compression
```

## Comparing `morley-0.0.4.tar` & `morley-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-03-16 13:47:16.507866 morley-0.0.4/
--rw-rw-rw-   0        0        0     6197 2023-03-16 13:47:16.507866 morley-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     5544 2022-12-22 08:51:42.000000 morley-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-03-16 13:47:16.498870 morley-0.0.4/morley/
--rw-rw-rw-   0        0        0    50022 2023-03-16 12:03:15.000000 morley-0.0.4/morley/Morley.py
--rw-rw-rw-   0        0        0        0 2022-10-12 08:40:07.000000 morley-0.0.4/morley/__init__.py
--rw-rw-rw-   0        0        0    84944 2022-11-30 16:54:03.000000 morley-0.0.4/morley/ethalon.png
--rw-rw-rw-   0        0        0    21968 2023-03-16 12:22:18.000000 morley-0.0.4/morley/gui.py
--rw-rw-rw-   0        0        0    17820 2022-11-30 16:54:03.000000 morley-0.0.4/morley/logo.png
--rw-rw-rw-   0        0        0     8255 2022-12-22 09:51:43.000000 morley-0.0.4/morley/main.py
--rw-rw-rw-   0        0        0      130 2023-03-16 12:29:49.000000 morley-0.0.4/morley/version.py
-drwxrwxrwx   0        0        0        0 2023-03-16 13:47:16.505871 morley-0.0.4/morley.egg-info/
--rw-rw-rw-   0        0        0     6197 2023-03-16 13:47:16.000000 morley-0.0.4/morley.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2023-03-16 13:47:16.000000 morley-0.0.4/morley.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-16 13:47:16.000000 morley-0.0.4/morley.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-03-16 13:47:16.000000 morley-0.0.4/morley.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       59 2023-03-16 13:47:16.000000 morley-0.0.4/morley.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-03-16 13:47:16.000000 morley-0.0.4/morley.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-16 13:47:16.508869 morley-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1626 2023-03-16 12:26:59.000000 morley-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 14:16:21.303643 morley-0.0.5/
+-rw-rw-rw-   0        0        0     6221 2023-07-06 14:16:21.303643 morley-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5544 2022-12-22 08:51:42.000000 morley-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 14:16:21.274739 morley-0.0.5/morley/
+-rw-rw-rw-   0        0        0    55571 2023-07-06 13:54:12.000000 morley-0.0.5/morley/Morley.py
+-rw-rw-rw-   0        0        0        0 2022-10-12 08:40:07.000000 morley-0.0.5/morley/__init__.py
+-rw-rw-rw-   0        0        0    84944 2022-11-30 16:54:03.000000 morley-0.0.5/morley/ethalon.png
+-rw-rw-rw-   0        0        0    22670 2023-05-30 14:12:12.000000 morley-0.0.5/morley/gui.py
+-rw-rw-rw-   0        0        0    17820 2022-11-30 16:54:03.000000 morley-0.0.5/morley/logo.png
+-rw-rw-rw-   0        0        0     9018 2023-05-30 12:13:25.000000 morley-0.0.5/morley/main.py
+-rw-rw-rw-   0        0        0      138 2023-05-11 21:09:23.000000 morley-0.0.5/morley/version.py
+drwxrwxrwx   0        0        0        0 2023-07-06 14:16:21.301649 morley-0.0.5/morley.egg-info/
+-rw-rw-rw-   0        0        0     6221 2023-07-06 14:16:21.000000 morley-0.0.5/morley.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2023-07-06 14:16:21.000000 morley-0.0.5/morley.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 14:16:21.000000 morley-0.0.5/morley.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-06 14:16:21.000000 morley-0.0.5/morley.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       59 2023-07-06 14:16:21.000000 morley-0.0.5/morley.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-06 14:16:21.000000 morley-0.0.5/morley.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-06 14:16:21.303643 morley-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1672 2023-05-11 21:09:23.000000 morley-0.0.5/setup.py
```

### Comparing `morley-0.0.4/PKG-INFO` & `morley-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: morley
-Version: 0.0.4
+Version: 0.0.5
 Summary: GUI software for plant morphometry
 Home-page: UNKNOWN
 Author: Daria Emekeeva & Lev Levitsky
 Author-email: dashabezik65@gmail.com
 License: License :: OSI Approved :: Apache Software License
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Intended Audience :: End Users/Desktop
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # Morley
 
 Morley is open-sourse software for plants morphometry: measuring sprouts, roots length, plants area. Morley github repository is [here](https://github.com/dashabezik/Morley)
 
 # Overview
```

### Comparing `morley-0.0.4/README.md` & `morley-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `morley-0.0.4/morley/Morley.py` & `morley-0.0.5/morley/Morley.py`

 * *Files 17% similar despite different names*

```diff
@@ -70,55 +70,53 @@
 # \- xlabel: str. The default is 'length, mm'
 #
 # \- param: str. Means the measured parameter (for ex. length, square, width).The default is 'length'
 
 # In[ ]:
 
 
- 
+
 
 def hist(tmp_l,tmp_r_max, tmp_r_sum,tmp_p, whiskers_dict, path_to_file_folder_fixed,path_to_output_dir, is_save = False, figname=None):
     fig, axes = plt.subplots(len(tmp_l.columns), 4, figsize=(35, 8*len(tmp_l.columns)))
     matplotlib.rcParams.update({'font.size': 20})
     param_type = 0
     fig.suptitle('X axis: Length, mm (root max, root sum and leaves); Area, mm2 (plant area);'
                  +'\n Y axis: Frequency, rel. units')
     param = ['leaves','roots_max','roots_sum', 'plant_area']
+    param_for_label = ['shoots','maximum_root','total_root', 'plant_surface_area']
     for tmp in [tmp_l,tmp_r_max, tmp_r_sum, tmp_p]:
         iterator = 0
 
         for g in tmp_l.columns:
-#             tmp[g] = tmp[tmp[g]>0][g]
             plt.subplot(len(tmp.columns), 4, param_type+4*iterator+1)
             mean = round(pd.Series(tmp[g].values.reshape(-1), dtype=np.float64).dropna().mean())
             ci = round(whiskers_dict[param[param_type]][g])
-            label = (str(param[param_type])+' '+str(g) +'\n'+
+            label = (str(param_for_label[param_type])+' '+str(g) +'\n'+
                      f'shapiro p-value = {scipy.stats.shapiro(pd.Series(tmp[g].values.reshape(-1), dtype=np.float64).dropna())[1]:.2e}'+
                     '\n'+'mean = '+str(mean)+'$\pm$'+str(ci))
 
             sns.histplot(pd.Series(tmp[tmp[g]< mean+3*max(mean,ci)][g].values.reshape(-1), dtype=np.float64).dropna(),
                      color=sns.color_palette("Set2")[iterator],
                                  label=label, kde = True)
             plt.xlim(left = 0, right = mean+3*max(mean,ci))
             plt.ylabel('')
-            light = mpatches.Patch(color=sns.color_palette("Set2")[param_type], label=r'{param}'.format(param =  param[param_type][0].upper()+param[param_type][1:]))
+            light = mpatches.Patch(color=sns.color_palette("Set2")[param_type], label=r'{param}'.format(param =  param_for_label[param_type][0].upper()+param_for_label[param_type][1:]))
             plt.legend(loc = 'upper right')
 
             iterator +=1
         param_type+=1
-#     plt.show()
     for ax in axes.flat:
         ax.set(xlabel='x-label', ylabel='y-label')
 
     if is_save:
         if figname is None:
             figname = pic_filename('hist','l_rm_rs',path_to_file_folder_fixed)
 #             report_area.insert(tk.END, str(path.join(path_to_output_dir,figname))+'\n')
         plt.savefig(path.join(path_to_output_dir,figname),bbox_inches = 'tight')
-#     plt.show()
 
 
 # ### Drop outliers
 #
 # Function drops values lying lower or upper than 25 or 75 quartille.
 
 
@@ -199,22 +197,22 @@
         ret = scipy.stats.mannwhitneyu(df1,df2, use_continuity = False ,alternative = 'two-sided')
     return ret
 
 def p_value_function (df, columns, is_norm):
     import scipy.stats as sps
     pvalue_table = pd.DataFrame(index = list(str(x) for x in columns.keys()),
                                 columns=list(str(x) for x in columns.keys()))
-    for i in (list(columns.keys())):
+    for i in (list(columns.keys())):  
         for j in (list(columns.keys())):
 #             a = pd.DataFrame(pd.Series(df[columns[i]].values.reshape(-1), dtype=np.float64).dropna())
-#             a = drop_outliers(a,a.columns)            
+#             a = drop_outliers(a,a.columns)
 #             b = pd.DataFrame(pd.Series(df[columns[j]].values.reshape(-1), dtype=np.float64).dropna())
 #             b = drop_outliers(b,b.columns)
 #             pvalue_table[str(i)].loc[str(j)] = pvalue_calc(a,b,is_norm)[1]
-            
+
             pvalue_table[str(i)].loc[str(j)] = pvalue_calc(pd.Series(df[columns[i]].values.reshape(-1), dtype=np.float64).dropna(),
                                                             pd.Series(df[columns[j]].values.reshape(-1), dtype=np.float64).dropna(),is_norm)[1]
     pvalue_table.fillna(value=1, inplace = True)
 
     return pvalue_table
 
 
@@ -256,91 +254,98 @@
 
 
 def pic_filename(plot_type, plant_param, path_to_folder):
     report_filename = (str(path.basename(path.normpath(path_to_folder)))+'_'+str(plant_param)+'_'+plot_type+
                              '_'+str(datetime.datetime.now().date())+'.jpg')
     return report_filename
 
-def bar_plot_function(l_or_r, df, columns, pv_table, path_to_file_folder_fixed, path_to_output_dir,
+def bar_plot_function(l_or_r, df, columns, pv_table, path_to_file_folder_fixed, path_to_output_dir, seed_circ_half_length,
                       is_save = False, figname=None,  union_DF_length = 500, xlabel = 'group label', ylabel = 'length, mm',
-                      param = 'length', auto_or_man = 'automatic',  is_drop_outliers = False):
+                      param = 'length', auto_or_man = 'automatic',  is_drop_outliers = False, is_norm = False):
     pv_tmp = pv_table.copy(deep=True)
-    print(pv_tmp)
     if type(columns)==dict:
         tmp = pd.DataFrame(columns=list(columns.keys()),index=np.arange(union_DF_length))
         for i in columns.keys():
-            tmp[i] = pd.DataFrame(pd.Series(df[columns[i]].values.reshape(-1), dtype=np.float64).dropna()) 
+            tmp[i] = pd.DataFrame(pd.Series(df[columns[i]].values.reshape(-1), dtype=np.float64).dropna())
         group_number_names = list(columns.keys())
     elif type(columns)==list: #### still 1D
         tmp = df
         group_number_names = columns ## если 2D массив, то range где кажд индекс +1 range(1, len(columns)+1)
     if is_drop_outliers:
-        tmp = drop_outliers(tmp, tmp.columns)         
+        tmp = drop_outliers(tmp, tmp.columns)
     c = sns.color_palette("Set2")
 
 
     matplotlib.rcParams.update({'font.size': 20})
-    fig, axes = plt.subplots(1, 2, figsize=(10, 5))
+    fig, axes = plt.subplots(1, 2, figsize=(10, 5), constrained_layout=True)
     fig.suptitle(r'{0}'.format(l_or_r[0].upper()+l_or_r[1:]))
     fig.tight_layout() #add space between subplots
 #     for i in list(tmp.columns):
 #         tmp[i] = pd.Series(tmp[i].values.reshape(-1)).dropna()
-    
+
 
     a = sns.barplot(ax = axes[0], data=tmp[group_number_names], palette=c)
     plt.xlabel(xlabel, fontsize = 20)
     plt.ylabel(ylabel, fontsize = 20)
-    
-    
+    plt.xticks(rotation =  90)
+    a.tick_params(axis = 'x', rotation = 90)
+
     for ax in axes.flat:
         ax.set( ylabel=ylabel)
 
     whiskers = defaultdict(type(group_number_names[0]))
     i=0
     for j in group_number_names:
         whiskers[j] = ((a.get_lines()[i].get_data()[1][1]-a.get_lines()[i].get_data()[1][0])/2)
         i+=1
-    
-    matplotlib.rcParams.update({'font.size': 20}) 
-    
+
+    matplotlib.rcParams.update({'font.size': 20})
+
     for i in list(pv_tmp.columns):
-        
+
         for j in list(pv_tmp.columns):
-            pv_tmp[str(i)].loc[str(j)] = scipy.stats.mannwhitneyu(tmp[i],tmp[j],
+            is_not_norm = not is_norm
+            method = is_norm*'Unpaired T-test'+is_not_norm*'Mann Whitney U-test'
+            if method=='Unpaired T-test':
+                pv_tmp[str(i)].loc[str(j)] = scipy.stats.ttest_ind(pd.Series(tmp[i].values.reshape(-1), dtype=np.float64).dropna(),
+                                                                  pd.Series(tmp[j].values.reshape(-1), dtype=np.float64).dropna())[1]
+            if method=='Mann Whitney U-test':
+                pv_tmp[str(i)].loc[str(j)] = scipy.stats.mannwhitneyu(pd.Series(tmp[i].values.reshape(-1), dtype=np.float64).dropna(),
+                                                                  pd.Series(tmp[j].values.reshape(-1), dtype=np.float64).dropna(),
                                                                  use_continuity = False ,alternative = 'two-sided')[1]
-        print(tmp[i])
-    print(pv_tmp)
 
     for i in range(0,pv_tmp.shape[1]):
         for j in range(0,pv_tmp.shape[1]):
             if i>j:
                 pv_tmp[pv_tmp.columns[i]].loc[pv_tmp.columns[j]] = np.nan
             elif pv_tmp[pv_tmp.columns[i]].loc[pv_tmp.columns[j]]>0.05:
                 pv_tmp[pv_tmp.columns[i]].loc[pv_tmp.columns[j]] = 1
-            elif pv_tmp[pv_tmp.columns[i]].loc[pv_tmp.columns[j]]<0.05:
+            elif ((pv_tmp[pv_tmp.columns[i]].loc[pv_tmp.columns[j]]<0.05)&
+            (abs(tmp[tmp.columns[j]].mean()- tmp[tmp.columns[i]].mean())>seed_circ_half_length)):
                 pv_tmp[pv_tmp.columns[i]].loc[pv_tmp.columns[j]] = 0.00003
-                
+
     f=np.array(pv_tmp, dtype='float64')
     color_def = [[0.247, 0.41176, 0.349],[0.624, 0.8967, 0.81]]
-    sns.heatmap(f, xticklabels=pv_tmp.columns, yticklabels=pv_tmp.columns, cbar=False, cmap = color_def, 
+    sns.heatmap(f, xticklabels=pv_tmp.columns, yticklabels=pv_tmp.columns, cbar=False, cmap = color_def,
                 ax = axes[1],vmin = 0, vmax = 1.5)
     dark = mpatches.Patch(color=color_def[0], label='p_value<0.05')
     light = mpatches.Patch(color=color_def[1], label='p_value>0.05')
     plt.legend(handles=[dark, light])
+    plt.yticks(rotation = 0)
 
     for ax in axes.flat:
         ax.set( xlabel=xlabel)
     axes[1].set(ylabel=xlabel) #heatplot has group label on y scale
-    
+    fig.tight_layout()
+
     if is_save:
         if figname is None:
             figname = pic_filename('bar',l_or_r.replace(' ', ''),path_to_file_folder_fixed)
 #             report_area.insert(tk.END, path.join(path_to_output_dir,figname)+'\n')
         plt.savefig(path.join(path_to_output_dir,figname),bbox_inches = 'tight')
-#     plt.show()
 
     return tmp, whiskers
 
 
 # ### Seed germination counter
 #
 # Function for counting the rate of non germinated seeds in all groups. The default value to consider the seed as nongerminated is 10 mm. If any root of leave has appropriate length, the seed is considered germinated (look at the table).
@@ -365,20 +370,20 @@
         if full_number:
             non_germinated_table[i].loc[0] = 1-(np.array((r<threshold))*np.array((l<threshold))).sum()/full_number
 
     fig = plt.figure()
     ax = fig.add_subplot(111)
     matplotlib.rcParams.update({'font.size': 20})
     plt.xlabel('Group label', fontsize = 20)
-    plt.ylabel('1-NG/TN', fontsize = 20)     
+    plt.ylabel('1-NG/TN', fontsize = 20)
     plt.xticks(fontsize = 20)
     plt.yticks(fontsize = 20)
     sns.barplot(x=non_germinated_table.columns, y = non_germinated_table.values[0],
                 palette=sns.color_palette("Set2"))
-    plt.title('Germination efficiency', fontsize=20)
+    plt.title('Germination rate', fontsize=20)
 
     if is_save:
         if figname is None:
             figname = pic_filename('bar','seed_germ',path_to_file_folder_fixed)
         plt.savefig(path.join(path_to_output_dir,figname),bbox_inches = 'tight')
 #     plt.show()
     return non_germinated_table
@@ -393,32 +398,36 @@
 def length(width, square, pixel):
     if (width!=0):
         length = square/(width*pixel)
     else:
         length = 0
     return length
 
+def seed_bias(length, width, roots_quantity, seed_length):
+    if (round(width)!=0):
+        length = length+seed_length*roots_quantity
+    return length
 
 # ### Folders_list_functions
 
 # Если папок для перечисления много, то можно вызвать функцию, которая скомпанует всё что лежит в папке в один лист
 
 # In[ ]:
 
 
 def folders_list_function(path_to_file_folder):
     folders_list=[]
     for filename_in_folder in listdir(path_to_file_folder):
         if path.isdir(path.join(path_to_file_folder,filename_in_folder)):
             folders_list.append(filename_in_folder)
+    not_needed_folders = ['.ipynb_checkpoints', 'template', 'color_block_separation', 'seeds_search', 'contours']
+    for folder in not_needed_folders:
+        if folder in folders_list:
+            folders_list.remove(folder)
 
-    if '.ipynb_checkpoints' in folders_list:
-        folders_list.remove('.ipynb_checkpoints')
-    if 'template' in folders_list:
-        folders_list.remove('template')
     return folders_list
 
 
 # ### files_dicts
 #
 # The function builds dicts with names of the columns in df, based on photos filenames. The main feachure is that all the columns names are merged by test groups names. Keys are the test groups names. Returns leaves_dict, roots_dict, roots_area_dict, plant_area_dict -- dicts with columns related to a specific test group.
 
@@ -431,37 +440,29 @@
     folders_list = folders_list_function(path_to_file_folder_fixed)
 
     leaves_dict = dict()
     for i in folders_list:
         leaves_dict[i] = []
 
     for g in folders_list:
-    #     pic_num=0
         path_to_file_folder = path_to_file_folder_fixed
         path_to_file_folder = path.join(path_to_file_folder, str(g)+'/')
         for filename_in_folder in listdir(path_to_file_folder):
-    #         pic_num +=1
-    #         if pic_num>3:
-    #             continue
             if filename_in_folder!='.ipynb_checkpoints':
                 file_name = path.join(path_to_file_folder, filename_in_folder)
                 leaves_dict[g].append('leaves_length_'+file_name)
 
     roots_dict = dict()
     for i in folders_list:
         roots_dict[i] = []
 
     for g in folders_list:
-    #     pic_num=0
         path_to_file_folder = path_to_file_folder_fixed
         path_to_file_folder = path.join(path_to_file_folder, str(g)+'/')
         for filename_in_folder in listdir(path_to_file_folder):
-    #         pic_num +=1
-    #         if pic_num>3:
-    #             continue
             if filename_in_folder!='.ipynb_checkpoints':
                 file_name = path.join(path_to_file_folder, filename_in_folder)
                 roots_dict[g].append('roots_length_'+file_name)
 
     roots_max_dict = dict()
     for i in folders_list:
         roots_max_dict[i] = []
@@ -506,24 +507,48 @@
 def pixel_color_conditions(pixel ,h1=0, h2=255, s1=0, s2=255, v1=0, v2=255):
     h, s, v = pixel # pixel = img_hsv[x, y]
     h_condition = (h>=h1)&(h<=h2)
     s_condition = (s>=s1)&(s<=s2)
     v_condition = (v>=v1)&(v<=v2)
     full_condition = h_condition*s_condition*v_condition
     return full_condition
-
-def drop_seeds(src, h1=0, h2=255, s1=0, s2=255, v1=0, v2=255):
-    src_hsv  = cv.cvtColor(src, cv.COLOR_BGR2HSV)
+ 
+def drop_seeds_old(src, h1=0, h2=255, s1=0, s2=255, v1=0, v2=255):
+    src_hsv  = cv.cvtColor(src, cv.COLOR_BGR2HSV) 
     h_min = np.array((h1, s1, v1), np.uint8)
     h_max = np.array((h2, s2, v2), np.uint8)
     tresh = cv.inRange(src_hsv, h_min, h_max)
     tresh=cv.bitwise_not(tresh)
     mask = cv.bitwise_or(src, src, mask=tresh)
     return mask
 
+def drop_seeds(src, contours, area_cont, h1=0, h2=255, s1=0, s2=255, v1=0, v2=255):
+    src_hsv  = cv.cvtColor(src, cv.COLOR_BGR2HSV)
+    h_min = np.array((h1, s1, v1), np.uint8)
+    h_max = np.array((h2, s2, v2), np.uint8)
+    thresh = cv.inRange(src_hsv, h_min, h_max)
+    mask = src.copy()
+#     thresh = np.clip(thresh, 0,1)
+    for i in range(len(contours)):
+        c = contours[i]
+        cimg1 = np.zeros_like(thresh)
+        cv.drawContours(cimg1, contours, i, color=255, thickness=-1)
+        
+        cimg1 = np.clip(cimg1, 0 ,1)
+        a = np.array(list(map(list,(zip(np.where(cimg1*thresh>0)[0],np.where(cimg1*thresh>0)[1])))))
+        a_cont = []
+        for i in range(len(a)):
+            a_cont.append([[a[i][1],a[i][0]]])
+        a_cont = np.array(a_cont)
+        mask = cv.bitwise_and(mask, mask, mask=cv.bitwise_not(cimg1*thresh))
+        if ((cimg1*thresh).sum()>0)&(len(a_cont)>5):
+            if np.prod(np.array((cv.fitEllipseDirect(a_cont)[1])))<2*area_cont:
+                cv.ellipse(mask, cv.fitEllipseDirect(a_cont),(0,0,0),-1)
+                cv.ellipse(mask, cv.fitEllipseDirect(a_cont),(0,0,0),10)
+    return mask
 
 # ### Linear approximation
 # After seed position search it is needed to find the line dividing leaves and roots.
 
 # In[ ]:
 
 
@@ -549,34 +574,26 @@
     src_hsv  = cv.cvtColor(src, cv.COLOR_BGR2HSV)
     h_min = np.array((h1, s1, v1), np.uint8)
     h_max = np.array((h2, s2, v2), np.uint8)
     thresh = cv.inRange(src_hsv, h_min, h_max)
     thresh = np.clip(thresh, 0,1)
     counter = np.zeros(len(contours))
     for i in range(len(contours)):
-        c = contours[i]
+        # c = contours[i]
         cimg1 = np.zeros_like(thresh)
         cv.drawContours(cimg1, contours, i, color=255, thickness=-1)
-#         plt.figure(figsize=(14,14))
-#         plt.imshow(cimg1)
-#         plt.show()
-#         plt.figure(figsize=(14,14))
-#         plt.imshow(thresh)
-#         plt.show()
-
-#         print('plant area = ', cv.contourArea(c) )
         cimg1 = np.clip(cimg1, 0 ,1)
         counter[i] = (cimg1*thresh).sum()
     return counter
 
 
 # ### Find_paper
 
 def find_paper(src, template_size, square_threshold, position_x_axes, ppm, canny_top=100, canny_bottom=10, morph=7, gauss=3):
-    
+
     # gr = cv.cvtColor(src, cv.COLOR_BGR2GRAY)
     bl = cv.GaussianBlur(src, (gauss,gauss), 0)
     canny = cv.Canny(bl, canny_bottom, canny_top)
     kernel = cv.getStructuringElement(cv.MORPH_ELLIPSE, (int(morph), int(morph)))
     closed = cv.morphologyEx(canny, cv.MORPH_CLOSE, kernel)
     contours0 = cv.findContours(closed.copy(), cv.RETR_EXTERNAL, cv.CHAIN_APPROX_SIMPLE)[0]
     # contours0 = contours0[0] if imutils.is_cv2() else contours0[1]
@@ -586,31 +603,27 @@
     for cont in contours0:
 #         cv.drawContours(src,[cont],0,(0,255,0),-2)
         center, radius = cv.minEnclosingCircle(cont)
         if (cv.contourArea(cont)>square_threshold)&(center[0]>position_x_axes): #position = src.shape[1]//8
             sm = cv.arcLength(cont, True)
             apd = cv.approxPolyDP(cont, 0.025*sm, True)
             center, radius = cv.minEnclosingCircle(cont)
-#             cv.drawContours(src, [cont], -1, (0,255,0), -2)
             if True:
                 # is_paper_founded = True
                 # paper = cont
                 cv.drawContours(src, [cont], -1, (0,255,0), -2)
                 pixelsPerMetric = 7.6
                 box = cv.minAreaRect(cont)
                 box = cv.boxPoints(box)
                 box = np.array(box, dtype="int")
                 (tl, tr, br, bl) = box
                 (tltrX, tltrY) = midpoint(tl, tr)
                 (blbrX, blbrY) = midpoint(bl, br)
                 (tlblX, tlblY) = midpoint(tl, bl)
                 (trbrX, trbrY) = midpoint(tr, br)
-                # dA = dist.euclidean((tltrX, tltrY), (blbrX, blbrY))
-                # dB = dist.euclidean((tlblX, tlblY), (trbrX, trbrY))
-    #             if (dB/template_size > (square_threshold/)):
                 pixelsPerMetric = math.sqrt(cv.contourArea(cont)/(template_size))
                 ppm.append(pixelsPerMetric)
             else:
                 pixelsPerMetric = ppm[-1]
 
             rect = cv.minAreaRect(apd)
             box = cv.boxPoints(rect) # поиск четырех вершин прямоугольника
@@ -625,19 +638,20 @@
 # ### Random file
 
 # In[ ]:
 
 
 def random_file(path_to_file_folder):
     a=random.choice(os.listdir(path_to_file_folder))
-    while (a=='template')|(a=='.ipynb_checkpoints'):
+    not_needed_folders_list = ['.ipynb_checkpoints', 'template', 'color_block_separation', 'seeds_search', 'contours']
+    while any(a==i for i in not_needed_folders_list):
         a=random.choice(os.listdir(path_to_file_folder))
     path_to_file = path.join(path_to_file_folder, a+'/')
     b = random.choice(os.listdir(path_to_file))
-    while (b=='.ipynb_checkpoints'):
+    while any(b==i for i in not_needed_folders_list):
         b=random.choice(os.listdir(path_to_file))
     path_to_file = path.join(path_to_file, b)
     return path_to_file
 
 
 # ### Class of parameters
 
@@ -657,25 +671,26 @@
 
 def add_annotation(name, text):
     with open(name, 'r+') as f:
         content = f.read()
         f.seek(0, 0)
         f.write(text)
         f.write(content)
-        
+
 def clean_table(df):
     d = defaultdict(str)
     for i in list(df.columns):
         a = re.split('/|\\||:|\\\\ ' ,i)
         try:
             d[i] = str(a[0]+'_'+a[-1])
         except:
             pass
     df.drop(columns = [i for i in list(df.columns) if 'width' in i ],axis = 1, inplace=True)
-    for j in ['roots_area_','leaves_area_','seed_area']:
+#     for j in ['roots_area_','leaves_area_','seed_area']:
+    for j in ['seed_area']:
         df.drop(columns = [i for i in list(df.columns) if i.startswith(j) ],axis = 1, inplace=True)
     df.rename(columns = d, inplace = True)
     return df
 
 
 def midpoint(ptA, ptB):
     return ((ptA[0] + ptB[0]) * 0.5, (ptA[1] + ptB[1]) * 0.5)
@@ -704,33 +719,48 @@
     rotate = gui.state['rotation'].get()
     path_to_file_folder_fixed = gui.state['paths']['input']
     path_to_output_dir = gui.state['paths']['out_dir']
     paper_area = gui.state['paper_area'].get()
     germ_thresh = gui.state['germ_thresh'].get()
     paper_area_threshold = gui.state['paper_area_thresold'].get()
     x_pos_divider = 11
-    indent_width_calc = gui.state['seed_margin_width'].get() #indent from the grain to calculate the width of the parts of the plants, so as not to take into account the width of the grain. For large grains and short sprouts, it is recommended to take a value of 10%; for small seeds, it is recommended to take a value of 100%.
+    is_seed_big = gui.state['is_seed_big'].get()
+    indent_width_calc = 10*(is_seed_big==1)+100*(is_seed_big==0) #indent from the grain to calculate the width of the parts of the plants, so as not to take into account the width of the grain. For large grains and short sprouts, it is recommended to take a value of 10%; for small seeds, it is recommended to take a value of 100%.
     contour_area_threshold = gui.CONTOUR_AREA_THRESHOLD # look at your img size and evaluate the threshold, 1000 is recomended
     template_filename = gui.state['paths']['template_file']
     hlb,hlt,slb,slt,vlb,vlt = get_state_values('leaves')
     hrb,hrt,srb,srt,vrb,vrt = get_state_values('roots')
     hsb,hst,ssb,sst,vsb,vst = get_state_values('seed')
     morph, gs, c_top = get_state_values('settings')
     c_bottom = 0
     ppm = [7.45]
-    
+
+        ### Plant contour ####
+    template = cv.imdecode(np.fromfile(template_filename, dtype=np.uint8), cv.IMREAD_COLOR)
+    template_hsv  = cv.cvtColor(template, cv.COLOR_BGR2HSV)
+    bl_t=cv.GaussianBlur(template,(5,5),0)
+    canny_t = cv.Canny(bl_t, 0, 140)
+    kernel_t = cv.getStructuringElement(cv.MORPH_ELLIPSE, (7,7))
+    closed_t = cv.morphologyEx(canny_t, cv.MORPH_CLOSE, kernel_t)
+    contours0_t = cv.findContours(closed_t.copy(), cv.RETR_EXTERNAL, cv.CHAIN_APPROX_SIMPLE)[0]
+    contour_area_threshold_index = np.array([cv.contourArea(cont) for cont in contours0_t]).argmax()
+    ellipse = cv.fitEllipse(contours0_t[contour_area_threshold_index])
+    contour_area_threshold = int(np.prod(np.array(ellipse[1]))/4)
+    seed_circ_half_length_in_pixels = math.sqrt(contour_area_threshold*3.14)
+    logger.info('Template area = '+str(contour_area_threshold))
+
     if 'color_block_separation' not in listdir(path_to_output_dir):
         os.mkdir(path.join(path_to_output_dir,'color_block_separation'))
-    if 'seeds_search' not in listdir(path_to_output_dir):
-        os.mkdir(path.join(path_to_output_dir,'seeds_search'))
+#     if 'seeds_search' not in listdir(path_to_output_dir):
+#         os.mkdir(path.join(path_to_output_dir,'seeds_search'))
     if 'contours' not in listdir(path_to_output_dir):
         os.mkdir(path.join(path_to_output_dir,'contours'))
-    
+
     # ppm - pixel per metric, массив с коэфам пересчета пикселя в мм, на случай плохого поиска стикера на фото
-    
+
     logger.info('Contour search parameters: %s', get_state_values('settings'))
     logger.info('Roots color, hsv parameters: %s', get_state_values('roots'))
     logger.info('Leaves color, hsv parameters: %s', get_state_values('leaves'))
 
     ###SEARCH###
     logger.info('SEARCH')
 
@@ -739,140 +769,161 @@
     folders_list = folders_list_function(path_to_file_folder_fixed)
     FL = len(folders_list)
 
     for g in folders_list:
         path_to_file_folder = path.join(path_to_file_folder_fixed, str(g)+'/')
         PL = len(listdir(path_to_file_folder))
         for filename_in_folder in listdir(path_to_file_folder):
+            if gui.state['abort_flag']:
+                logger.critical('SEARCH ABORTED.')
+                return
             Progress_bar_value += 90 // (PL * FL)
             gui.state['progress'].set(Progress_bar_value)
-            # pb.configure(value = Progress_bar_value)
-            # pb_lbl['text'] = str(round(Progress_bar_value))+'%'
-            # pb.update()
-            # pb_lbl.update()
             if filename_in_folder=='.ipynb_checkpoints':
                 continue
             ### CONTOURS ###
             logger.info('File name: %s', filename_in_folder)
             logger.info('LOOKING FOR CONTOURS ...')
 
             file_name = path.join(path_to_file_folder, filename_in_folder)
-
-            ### Plant contour ####
-
-            #src = cv.imread(file_name)
             src = cv.imdecode(np.fromfile(file_name, dtype=np.uint8), cv.IMREAD_COLOR)
             src = gui.rotate_pic(src, rotate)
             gr = cv.cvtColor(src, cv.COLOR_BGR2GRAY)
             bl=cv.GaussianBlur(src,(gs,gs),0)
             canny = cv.Canny(bl, c_bottom, c_top)
             kernel = cv.getStructuringElement(cv.MORPH_ELLIPSE, (morph,morph))
             closed = cv.morphologyEx(canny, cv.MORPH_CLOSE, kernel)
             contours0 = cv.findContours(closed.copy(), cv.RETR_EXTERNAL, cv.CHAIN_APPROX_SIMPLE)[0]
             # contours0 = contours0[0] if imutils.is_cv2() else contours0[1]
             (contours0, _) = contours.sort_contours(contours0)
             pixelsPerMetric = None
             quantity_of_plants = 0
             real_conts = []
 
+
+
             pixelsPerMetric, ppm = find_paper(src, paper_area, paper_area_threshold, position_x_axes(src,x_pos_divider), ppm,
                                          canny_top=c_top, canny_bottom=c_bottom,morph=morph)
-            
+
+            seed_circ_half_length = seed_circ_half_length_in_pixels/pixelsPerMetric
+
+            logger.info('Seeds circularity length, mm: ' + str(round(seed_circ_half_length)))
+
             i=0
             src_to_save = src.copy()
             for cont in contours0:
                 if (cv.contourArea(cont)>contour_area_threshold):
                     center, radius = cv.minEnclosingCircle(cont) #recomended range of plants position is between 1/3 and 2/3
                     if ((cv.contourArea(cont) > contour_area_threshold)&
                         (center[0] > src.shape[1]//3)&(center[0] < src.shape[1]*2//3)):
                         real_conts.append(cont)
                         left = tuple(cont[cont[:, :, 0].argmin()][0])
                         cv.drawContours(src_to_save,[cont],0,(255,255,5),2)
                         cv.putText(src_to_save, "%s" %(i,), (left[0] - 10, left[1]-10), cv.FONT_HERSHEY_SIMPLEX, 4, (255, 255, 2), 4)
                         i+=1
-            #                     cv.drawContours(src,[cont],0,(255,255,5),2)
-            cv.imwrite(path.join(path_to_output_dir,'contours',filename_in_folder.split('.')[0]+'_contours.jpg'), src_to_save)
-            
+            script_path = os.getcwd()
+            os.chdir(path_to_output_dir)
+            cv.imwrite(path.join('contours','.'.join(filename_in_folder.split('.')[:-1])+'_contours.jpg'), src_to_save)
+            os.chdir(script_path)
             quantity_of_plants = len(real_conts)
             logger.info('Quantity of plants: %d', quantity_of_plants)
             logger.info('Pixels per metric: %.3f', pixelsPerMetric)
 
-            ### SEEDS ###
+           
+        
+        ##################################### OLD #########################################
+        
+        ### SEEDS ###
             logger.info('LOOKING FOR SEEDS POSITION ...')
 
 #             img2 = cv.imread(file_name,0)
             img2 = cv.imdecode(np.fromfile(file_name, dtype=np.uint8), cv.IMREAD_COLOR)
             img2 = gui.rotate_pic(img2, rotate)
             img2 = cv.cvtColor(img2, cv.COLOR_BGR2GRAY)
 #             template = cv.imread(template_filename,0)
             template = cv.imdecode(np.fromfile(template_filename, dtype=np.uint8), cv.IMREAD_COLOR)
             template = gui.rotate_pic(template, rotate)
             template = cv.cvtColor(template, cv.COLOR_BGR2GRAY)
             w, h = template.shape[::-1]
 
 
-            methods = ['cv.TM_CCOEFF_NORMED']
-            for meth in methods:
-                img = img2.copy()
-                method = eval(meth)
-                # Apply template Matching
-                res = cv.matchTemplate(img,template,method)
-                threshold = 0.55
-                loc = np.where( res > threshold)
-                x=np.array([])
-                y=np.array([])
-                for pt in zip(*loc[::-1]):
-                    if (pt[0] > src.shape[1]/3)&((pt[0] < 2*src.shape[1]/3)):
-                        cv.rectangle(img, pt, (pt[0] + w, pt[1] + h), (0,0,255), 5)
-                        x=np.append(x,pt[0])
-                        y=np.append(y,pt[1])
-                slope, intercept = linear_approx(y,x)
-                
-                
-                p1 = [int(intercept)-int(w*indent_width_calc/100),0]
-                p2 = [int(slope*img.shape[0]+intercept)-int(w*indent_width_calc/100),img.shape[0]]
-                pts_leaves = np.array([[0,0],p1,p2,[0,img.shape[0]]])
-                pts_roots = np.array([[p1[0]+3*w//4+int(w*indent_width_calc/100),p1[1]],[p2[0]+3*w//4+int(w*indent_width_calc/100),p2[1]],[img.shape[1],img.shape[0]],[img.shape[1],0]])
-                
-                cv.imwrite(path.join(path_to_output_dir,'seeds_search',filename_in_folder.split('.')[0]+'_seeds_search.jpg'),img)
-           
-            Mode =pd.Series(x).mode()[0]   
-            mean_left_x = int(Mode)-w//4
-            mean_right_x = int(Mode) + 3*w//4
-            mean_left_x = round(mean_left_x)
-            mean_right_x = round(mean_right_x)
-            
-            src = drop_seeds(src,hsb,hst,ssb,sst,vsb,vst)
+##################################### OLD #########################################
+        
+        
+            src = drop_seeds(src,real_conts, contour_area_threshold,hsb,hst,ssb,sst,vsb,vst)
             src_black_seeds = src.copy()
             src_black_seeds = cv.cvtColor(src_black_seeds, cv.COLOR_BGR2HSV)
+            
+            
+#             os.chdir(path_to_output_dir)
+#             cv.imwrite(path.join('color_block_separation','.'.join(filename_in_folder.split('.')[:-1])+'_black_seed.jpg'), src_black_seeds)
+#             os.chdir(script_path)
+            
+            ##### NEW ######
+            h_min = np.array((0, 0, 0), np.uint8)
+            h_max = np.array((0, 0, 0), np.uint8)
+            thresh = cv.inRange(src_black_seeds, h_min, h_max)
+            thresh = np.clip(thresh, 0,1)
+            x = np.where(thresh ==1)[0]
+            y = np.where(thresh ==1)[1]
+            x = x[(y > src.shape[1]/3)&((y < 2*src.shape[1]/3))]
+            y = y[(y > src.shape[1]/3)&((y < 2*src.shape[1]/3))]
+            
+            mymodel = np.poly1d(np.polyfit(x, y, 3))
+
+            myline = np.linspace(1, src.shape[0], 100)
+
+            p1 = [mymodel(0),0]
+            p2 = [mymodel(src.shape[0]),src.shape[0]]
+            pts_leaves = np.array([[0,0]]+list(map(list,zip( map(int,mymodel(myline)-w*is_seed_big/2), map(int,myline))))+[[0,src.shape[0]]])
+            pts_roots = np.array(list(map(list,zip(map(int,mymodel(myline)+w*is_seed_big/2), map(int,myline))))+[[src.shape[1],src.shape[0]]]+[[src.shape[1],0]])
+
+            k,b = linear_approx(x, y)
+#             p1 = [int(b),0]
+#             p2 = [int(k*img.shape[0]+b),img.shape[0]]
+#             pts_leaves = np.array([[0,0],p1,p2,[0,img.shape[0]]])
+#             pts_roots = np.array([[p1[0]+3*w//4,p1[1]],[p2[0]+3*w//4,p2[1]],[img.shape[1],img.shape[0]],[img.shape[1],0]])
+            ##### NEW ######
+            
+            
+            
+            
             ### COLOR ###
             logger.info('MAKING COLOR ...')
 
             overlay = src.copy()
             cv.drawContours(overlay, [pts_leaves], -1,(0,224,79), -1)
             opacity = 0.25
             cv.drawContours(overlay, [pts_roots], -1, (240,0,255), -5)
             cv.addWeighted(overlay, opacity, src, 1 - opacity, 0, src)
             bl = cv.medianBlur(src, 7)
             bl=cv.GaussianBlur(bl,(5,   5),0)
-            cv.imwrite(path.join(path_to_output_dir,'color_block_separation',filename_in_folder.split('.')[0]+ '_color_block_separation.jpg'), src)
+            script_path = os.getcwd()
+
+            os.chdir(path_to_output_dir)
+            cv.imwrite(path.join('color_block_separation','.'.join(filename_in_folder.split('.')[:-1])+'_color_block_separation.jpg'), src)
+            os.chdir(script_path)
+            
+          
+
             img_hsv = cv.cvtColor(bl, cv.COLOR_BGR2HSV)
 #             cv.imwrite('colored/{0}'.format(filename_in_folder), src)
 #             mean_right_x = max(p1[0],p2[0])+3*w//4
 #             mean_left_x = min(p1[0],p2[0])
-            logger.info("Mean left seeds x-coordinate %d", mean_left_x)
-            logger.info("Mean right seeds x-coordinate %d", mean_right_x)
+#             logger.info("Mean left seeds x-coordinate %d", mean_left_x)
+#             logger.info("Mean right seeds x-coordinate %d", mean_right_x)
             ## WIDTH ###
             logger.info('WIDTH CALCULATION...')
 
             measure = pd.DataFrame(columns=['roots_area_{0}'.format(file_name), 'leaves_area_{0}'.format(file_name),
                                             'roots_length_{0}'.format(file_name), 'leaves_length_{0}'.format(file_name),
                                             'roots_width_{0}'.format(file_name), 'leaves_width_{0}'.format(file_name),
                                            'plant_area_{0}'.format(file_name),'seed_area_{0}'.format(file_name),
-                                           'roots_max_length_{0}'.format(file_name),'roots_max_width_{0}'.format(file_name)],
+                                           'roots_max_length_{0}'.format(file_name),'roots_max_width_{0}'.format(file_name),
+                                           'roots_quantity_{0}'.format(file_name), 'leaves_to_seeds_{0}'.format(file_name)],
                                    index=np.arange(len(real_conts)))
 
 
             for i in range(quantity_of_plants):
                 is_first = True
                 is_first_r = True
                 is_first_r_max = True
@@ -882,14 +933,20 @@
                 ramount = 0
                 r_max_amount = 0
                 c = real_conts[i]
                 left = tuple(c[c[:, :, 0].argmin()][0])
                 right = tuple(c[c[:, :, 0].argmax()][0])
                 top = tuple(c[c[:, :, 1].argmin()][0])
                 bottom = tuple(c[c[:, :, 1].argmax()][0])
+                
+                mean_left_x = int(mymodel(0.5*(top[1]+bottom[1])))
+                mean_right_x = int(mymodel(0.5*(top[1]+bottom[1]))+3*w/4)
+#                 logger.info("Mean left seeds x-coordinate %d", mean_left_x)
+#                 logger.info("Mean right seeds x-coordinate %d", mean_right_x)
+                
                 cv.line(img_hsv, left, right, (255, 255, 255), thickness=2)
                 step = (right[0]-mean_right_x)//3
                 if (mean_left_x-left[0])//3!=0:
                     for y in range(left[0],int(mean_left_x-w*indent_width_calc/100),(mean_left_x-left[0])//3):
                         is_first = True
                         for x in range(top[1],bottom[1]):#иттерация по вертикали, т к img.shape => (height, width), но компонента контура (х,у)
                             h, s, v = img_hsv[x, y]
@@ -908,27 +965,29 @@
                 # r_max_amaunt - счетчик для максимальной длины корня, ramount - для суммарной длины
 
                 if step!=0:
 
                     for y in range(int(mean_right_x+w*indent_width_calc/100), right[0],step):#идем по ввертикальным линиям
                         is_first_r = True
                         is_first_r_max = True
+                        N_roots_counter = np.array([]) # roots quantity in each vertical section
                         for x in range(top[1],bottom[1]):#иттерация по вертикали, т к img.shape => (height, width), но компонента контура (х,у)
                             h, s, v = img_hsv[x, y]
                             if (cv.pointPolygonTest(real_conts[i],(x,y), False)):# если точка внутри контура
                                 if (v>vrb)&((h>hrb)&(h<hrt)):# если эта точка = корень, а не фон
                                     ramount = ramount + 1*is_first_r#если это первое вхождение корня, то число корней+=1
                                     r_max_amount=r_max_amount+1*is_first_r_max
                                     is_first_r_max = False
                                     is_first_r = False#далее вхождение уже не первое
                                     roots += 1#число пикселей +=1
                                 else:
                                     is_first_r = True #если это не корень а фон, то вхождения нет
                             else:
                                 is_first_r = True#если это не в контуре, то вхождения точно нет
+                            N_roots_counter = np.append(N_roots_counter, ramount)
                 if (lamount == 0.0)|(lamount == 0):
                     leaves_width = 0
                 else:
                     leaves_width = leaves/lamount
 
                 if (ramount == 0.0)|(ramount == 0)|(step == 0):
                     roots_width = 0
@@ -936,84 +995,95 @@
                 else:
                     roots_width = roots/ramount
                     roots_max_width = roots/r_max_amount
 
                 measure['roots_width_{0}'.format(file_name)].iloc[i] = roots_width
                 measure['roots_max_width_{0}'.format(file_name)].iloc[i] = roots_max_width
                 measure['leaves_width_{0}'.format(file_name)].iloc[i]= leaves_width
+                measure['roots_quantity_{0}'.format(file_name)].iloc[i]= N_roots_counter.max()
 
             ### PIXEL COUNTING ###
             logger.info('PIXEL COUNTING ...')
 
 #             for i in range(len(real_conts)):
 #                 c = real_conts[i]
 #                 measure.iloc[i]['plant_area_{0}'.format(file_name)] = cv.contourArea(c)
 #                 print(cv.contourArea(c))
     #             measure.iloc[i]['seed_area_{0}'.format(file_name)] = seed_area
+
+    ### Calculation ###
             measure['leaves_area_{0}'.format(file_name)] =color_range_counter(src, real_conts, hlb,hlt,slb,slt,vlb,vlt)
             measure['roots_area_{0}'.format(file_name)] =color_range_counter(src, real_conts, hrb,hrt,srb,srt,vrb,vrt)
             measure['seed_area_{0}'.format(file_name)] =color_range_counter(src_black_seeds, real_conts, 0,1,0,1,0,1)
             measure['plant_area_{0}'.format(file_name)] = color_range_counter(src, real_conts, 0,255,0,255,vrb,255)
             measure['plant_area_{0}'.format(file_name)] = measure.apply(lambda x: x['plant_area_{0}'.format(file_name)]/(pixelsPerMetric*pixelsPerMetric), axis = 1 )
             measure['roots_length_{0}'.format(file_name)] = measure['roots_area_{0}'.format(file_name)]
             measure['leaves_length_{0}'.format(file_name)] = measure['leaves_area_{0}'.format(file_name)]
-
+    ### To mm ###
             measure['roots_length_{0}'.format(file_name)] = measure.apply(lambda x: length(x['roots_width_{0}'.format(file_name)],x['roots_area_{0}'.format(file_name)],pixelsPerMetric), axis = 1 )
             measure['roots_max_length_{0}'.format(file_name)] = measure.apply(lambda x: length(x['roots_max_width_{0}'.format(file_name)],x['roots_area_{0}'.format(file_name)],pixelsPerMetric), axis = 1 )
             measure['leaves_length_{0}'.format(file_name)] = measure.apply(lambda x: length(x['leaves_width_{0}'.format(file_name)],x['leaves_area_{0}'.format(file_name)],pixelsPerMetric), axis = 1 )
-            measure_full2 = measure_full2.join(measure, how = 'outer')
-
-            # plt.figure(figsize = (14,14))
-#             plt.imshow(src)
-#             plt.show()
+            measure['leaves_area_{0}'.format(file_name)] = measure.apply(lambda x: x['leaves_area_{0}'.format(file_name)]/(pixelsPerMetric*pixelsPerMetric), axis = 1 )
+            measure['roots_area_{0}'.format(file_name)] = measure.apply(lambda x: x['roots_area_{0}'.format(file_name)]/(pixelsPerMetric*pixelsPerMetric), axis = 1 )
+            measure['leaves_width_{0}'.format(file_name)] = measure.apply(lambda x: x['leaves_width_{0}'.format(file_name)]/(pixelsPerMetric), axis = 1 )
+            measure['roots_max_width_{0}'.format(file_name)] = measure.apply(lambda x: x['roots_max_width_{0}'.format(file_name)]/(pixelsPerMetric), axis = 1 )
+            measure['roots_width_{0}'.format(file_name)] = measure.apply(lambda x: x['roots_width_{0}'.format(file_name)]/(pixelsPerMetric), axis = 1 )
+
+    ### Add seed bias ###
+            measure['leaves_length_{0}'.format(file_name)] = measure.apply(lambda x: seed_bias(x['leaves_length_{0}'.format(file_name)], x['leaves_width_{0}'.format(file_name)], 1,seed_circ_half_length),axis = 1)
+            measure['roots_max_length_{0}'.format(file_name)] = measure.apply(lambda x: seed_bias(x['roots_max_length_{0}'.format(file_name)], x['roots_max_width_{0}'.format(file_name)], 1,seed_circ_half_length),axis = 1)
+            measure['roots_length_{0}'.format(file_name)] =measure.apply(lambda x: seed_bias(x['roots_length_{0}'.format(file_name)], x['roots_width_{0}'.format(file_name)], x['roots_quantity_{0}'.format(file_name)],seed_circ_half_length),axis = 1 )
+            measure['leaves_to_seeds_{0}'.format(file_name)] = measure['leaves_area_{0}'.format(file_name)]*pixelsPerMetric/contour_area_threshold
 
+            measure_full2 = measure_full2.join(measure, how = 'outer')
 
-            # files_frame.update_idletasks()
-            # files_frame.update()
-
-    del res,bl,overlay, img, img2, img_hsv, gr, canny, src, closed, src_black_seeds
+    del bl,overlay, img2, img_hsv, gr, canny, src, closed, src_black_seeds
 
-    measure_full2.to_csv(path.join(path_to_output_dir,'measure.csv'))
+    measure_full2.to_csv(path.join(path_to_output_dir,'measure_'+str(datetime.datetime.now().date())+'.csv'))
 
     dicts = files_dicts(path_to_file_folder_fixed)
     roots_sum_dict, roots_max_dict, plant_area_dict, leaves_dict = dicts.values()
     seed_germ = seed_germination(measure_full2, roots_max_dict.keys(), path_to_file_folder_fixed = path_to_file_folder_fixed,
                                  path_to_output_dir = path_to_output_dir, threshold=germ_thresh, is_save=True)
 
     shap =shapiro_test(measure_full2, dicts)
     plant_parameters = ['roots_sum','roots_max','plant_area','leaves']
     v= [0,0,0,0]
     p_value_dict = dict(zip(plant_parameters, v))
-    for i in plant_parameters:
-        is_not_norm = any(shap[i]<0.05)
-        is_norm = not is_not_norm
-        test_type = 'test_type = '+str(is_norm*'Unpaired T-test'+is_not_norm*'Mann Whitney U-test')+'\n' +'\n'
+#     for i in plant_parameters:
+#         is_not_norm = any(shap[i]<0.05)
+#         is_norm = not is_not_norm
+#         test_type = 'test_type = '+str(is_norm*'Unpaired T-test'+is_not_norm*'Mann Whitney U-test')+'\n' +'\n'
+
 
-        p_value_dict[i] = (p_value_function(measure_full2, dicts[i],is_norm),test_type)
-    
-    
     whiskers_dict = {'roots_sum': {},
                    'roots_max': {},
                    'plant_area': {},
                    'leaves': {}}
     result_dict = {'roots_sum': '',
                    'roots_max': '',
                    'plant_area': '',
                    'leaves': '',
                   'full_file_photo_separated': measure_full2}
-    plots_titles = {'roots_sum': 'Total roots length',
-               'roots_max': 'Maximal root length',
-               'plant_area': 'Plant surface area',
-               'leaves': 'Shoot length'}
+    plots_titles = {'roots_sum': 'Total roots',
+               'roots_max': 'Maximum root',
+               'plant_area': 'Plant surface',
+               'leaves': 'Shoot'}
 
     for i in whiskers_dict.keys():
+        is_not_norm = any(shap[i]<0.05)
+        is_norm = not is_not_norm
+        test_type = 'test_type = '+str(is_norm*'Unpaired T-test'+is_not_norm*'Mann Whitney U-test')+'\n' +'\n'
+        p_value_dict[i] = (p_value_function(measure_full2, dicts[i],is_norm),test_type)
+
         ylabel = 'length, mm'*(i!='plant_area')+'area, mm2'*(i=='plant_area')
         result_dict[i], whiskers_dict[i] = bar_plot_function(plots_titles[i], measure_full2, dicts[i], p_value_dict[i][0], ylabel=ylabel,
                                   path_to_file_folder_fixed = path_to_file_folder_fixed, path_to_output_dir = path_to_output_dir,
-                                                             is_save= True, union_DF_length=250,is_drop_outliers=True)
+                                  seed_circ_half_length = seed_circ_half_length, is_save= True, union_DF_length=250,
+                                                             is_drop_outliers=True, is_norm = is_norm)
 
     hist(result_dict['leaves'],result_dict['roots_max'], result_dict['roots_sum'],result_dict['plant_area'],
      whiskers_dict, path_to_file_folder_fixed = path_to_file_folder_fixed, path_to_output_dir = path_to_output_dir, is_save = True)
 
     report_information = ('Date and time: ' + str(datetime.datetime.now())+'\n'+
                       'Program settings and initial information: \n'+
                       'path_to_file_folder_fixed = '+ str(path_to_file_folder_fixed)+'\n'+
@@ -1021,17 +1091,17 @@
                       'paper threshold position = photo width/x_pos_divider = img.shape[0]/'+str(x_pos_divider)+'\n'+
                       'contour_area_threshold = '+str(contour_area_threshold)+' pixels \n'+
                       'template_filename = '+str(template_filename)+'\n'+
                       'leaves parameters'+ str(get_state_values('leaves')) +'\n'+
                       'roots parameters'+str(get_state_values('roots'))+'\n'+
                       'seeds parameters'+str(get_state_values('seed'))+'\n'+
                       'blur parameters'+str(get_state_values('settings'))+'\n' +'\n' )
-    
+
     result_dict['full_file_photo_separated'] = clean_table(measure_full2)
-    
+
     for i in result_dict.keys():
         report_table_filename = str(path.basename(path.normpath(path_to_file_folder_fixed)))+'_'+str(i)+'_'+str(datetime.datetime.now().date())+'.csv'
         result_dict[i].to_csv(path.join(path_to_output_dir,report_table_filename))
 
         with open(path.join(path_to_output_dir,report_table_filename), 'r+') as f:
             content = f.read()
             f.seek(0, 0)
@@ -1059,8 +1129,8 @@
     # pb_lbl.update()
     # pb.update()
     Progress_bar_value = 100
     gui.state['progress'].set(Progress_bar_value)
     logger.info('SEARCH FINISHED.')
     logger.info('Go to the output directory to see the result')
     # files_frame.update_idletasks()
-    # files_frame.update()
+    # files_frame.update()
```

### Comparing `morley-0.0.4/morley/ethalon.png` & `morley-0.0.5/morley/ethalon.png`

 * *Files identical despite different names*

### Comparing `morley-0.0.4/morley/gui.py` & `morley-0.0.5/morley/gui.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,636 +1,655 @@
-import tkinter as tk
-from tkinter.filedialog import askopenfilename, askdirectory, asksaveasfilename
-from PIL import ImageTk, Image
-import cv2 as cv
-import imutils
-from imutils import contours
-import numpy as np
-import pandas as pd
-import os
-import random
-from functools import partial
-import json
-import logging
-
-
-state = {
-    'settings': {
-        'morph': 5,
-        'gauss': 3,
-        'canny_top': 160
-    },
-    'color': {
-        'h_bottom': 50,
-        'h_top': 255,
-        's_bottom': 0,
-        's_top': 255,
-        'v_bottom': 100,
-        'v_top': 255,
-    },
-    'roots': {
-        'h_bottom': 0,
-        'h_top': 255,
-        's_bottom': 0,
-        's_top': 255,
-        'v_bottom': 0,
-        'v_top': 255,
-    },
-    'leaves': {
-        'h_bottom': 0,
-        'h_top': 255,
-        's_bottom': 0,
-        's_top': 255,
-        'v_bottom': 0,
-        'v_top': 255,
-    },
-    'seed': {
-        'h_bottom': 0,
-        'h_top': 20,
-        's_bottom': 100,
-        's_top': 255,
-        'v_bottom': 100,
-        'v_top': 255,
-    },
-    'paths': {
-        'out_dir': os.getcwd()
-    },
-    'rotation': 0,
-    'paper_area_thresold': 5000,
-    'paper_area': 0,
-    'germ_thresh': 10,
-    'progress': 0,
-    'seed_margin_width':100
-}
-
-STATE_SYNTAX_VERSION = 1
-STATE_SYNTAX_VERSION_KEY = 'syntax_version'
-CONTOUR_AREA_THRESHOLD = 1000
-FORMAT='{:.0f}'
-
-class FormatLabel(tk.Label):
-
-    def __init__(self, master=None, cnf={}, **kw):
-
-        # default values
-        self._format = FORMAT
-        self._textvariable = None
-        self.two_n_plus1 = None
-
-        # get new format and remove it from `kw` so later `super().__init__` doesn't use them (it would get error message)
-        if 'format' in kw:
-            self._format = kw['format']
-            del kw['format']
-
-        # get `textvariable` to assign own function which set formatted text in Label when variable change value
-        if 'textvariable' in kw:
-            self._textvariable = kw['textvariable']
-            self._trace_id = self._textvariable.trace('w', self._update_text)
-            del kw['textvariable']
-
-        # run `Label.__init__` without `format` and `textvariable`
-        super().__init__(master, cnf={}, **kw)
-
-        # update text after running `Label.__init__`
-        if self._textvariable:
-            #self._update_text(None, None, None)
-            self._update_text(self._textvariable, '', 'w')
-
-    def _update_text(self, a, b, c):
-        """update text in label when variable change value"""
-        self["text"] = self._format.format(self._textvariable.get())
-
-    def destroy(self):
-        self._textvariable.trace_vdelete('w', self._trace_id)
-        super().destroy()
-
-
-class LoggingToGUI(logging.Handler):
-    # https://stackoverflow.com/a/18194597/1258041
-    def __init__(self, console):
-        logging.Handler.__init__(self)
-        self.console = console
-
-    def emit(self, message):
-        formattedMessage = self.format(message)
-
-        self.console.configure(state=tk.NORMAL)
-        self.console.insert(tk.END, formattedMessage + '\n')
-        self.console.configure(state=tk.DISABLED)
-        self.console.see(tk.END)
-
-
-def save_state(fname):
-    state_dict = pythonize_state_dict()
-    for k in ['template', 'img_arr', 'img_arr_0', 'progress']:
-        state_dict.pop(k, None)
-    state_dict[STATE_SYNTAX_VERSION_KEY] = STATE_SYNTAX_VERSION
-    with open(fname, 'w') as f:
-        json.dump(state_dict, f)
-
-
-def update_dict(old, new):
-    for k, v in new.items():
-        if isinstance(v, dict):
-            update_dict(old[k], v)
-        elif k in old and hasattr(old[k], 'set'):
-            old[k].set(v)
-        else:
-            old[k] = v
-
-
-def load_state(fname, label_dict):
-    with open(fname) as f:
-        d = json.load(f)
-    update_dict(state, d)
-    set_state_variables(state)
-    update_labels(label_dict)
-    conditions.check_conditions()
-    conditions.update_conditions()
-
-
-def load_state_headless(fname):
-    set_state_variables(state, headless=True)
-    with open(fname) as f:
-        d = json.load(f)
-    update_dict(state, d)
-
-
-def update_labels(label_dict):
-    inp = state.get('paths', {}).get('input')
-    if inp:
-        set_label('input', label_dict['input'], inp)
-
-    template = state.get('paths', {}).get('template_file')
-    if template:
-        read_template_file(template, label_dict['template'])
-
-    outdir = state.get('paths', {}).get('out_dir')
-    if outdir:
-        set_label('outdir', label_dict['outdir'], outdir)
-
-    rotate = state.get('rotation')
-    if rotate:
-        set_label('rotation', label_dict['rotation'], rotate)
-
-
-def set_label(kind, label, value):
-    mapping = {
-        'input': lambda fname: f'Selected image directory: {os.path.basename(fname)}.',
-        'template': lambda fname: f'Selected seed template: {os.path.basename(fname)}.',
-        'outdir': lambda fname: f'Output directory: {os.path.basename(fname)}.',
-        'rotation': lambda angle: f'Rotation angle: {angle.get()}.'
-    }
-    label['text'] = mapping[kind](value)
-
-
-def load_state_dialog(label_dict):
-    fname = askopenfilename(title="Load settings...", filetypes=[('JSON files', '*.json'), ('All files', '*')])
-    if fname:
-        load_state(fname, label_dict)
-
-
-def save_state_dialog():
-    fname = asksaveasfilename(title="Save settings as...", defaultextension='.json')
-    if fname:
-        save_state(fname)
-
-
-class ConditionManager:
-    CONDITIONS = {
-        'rotate': ['input'],
-        'tweak': ['input', 'template'],
-        'run': ['input', 'template', 'paper_area', 'germ_thresh']
-    }
-    def __init__(self):
-        self.satisfied = set()
-
-    def register(self, widgets):
-        self.widgets = widgets
-        for k, w in widgets.items():
-            if k in self.CONDITIONS:
-                for widget in w:
-                    widget['state'] = tk.DISABLED
-
-    def satisfies(self, condition):
-        """Decorator that makes a function call satisfy the corresponding condition.
-        Changes the status of widgets after a successful call."""
-        def decorator(func):
-            def wrapped(*args, **kwargs):
-                ret = func(*args, **kwargs)
-                if ret:
-                    self.satisfied.add(condition)
-                    self.update_conditions()
-                return ret
-            return wrapped
-        return decorator
-
-    def update_conditions(self):
-        for key, v in self.CONDITIONS.items():
-            if all(w in self.satisfied for w in v) and key in self.widgets:
-                status = tk.NORMAL
-            else:
-                status = tk.DISABLED
-            for w in self.widgets[key]:
-                w['state'] = status
-
-    def check_conditions(self):
-        if state.get('paths', {}).get('input'):
-            self.satisfied.add('input')
-        if state.get('paths', {}).get('template_file'):
-            self.satisfied.add('template')
-        if state.get('paper_area').get():
-            self.satisfied.add('paper_area')
-        if state.get('germ_thresh').get():
-            self.satisfied.add('germ_thresh')
-
-
-conditions = ConditionManager()
-
-
-def trace_entry(key):
-    def callback(name, index, op):
-        try:
-            assert state[key].get() != 0
-        except (AssertionError, tk.TclError):
-            if key in conditions.satisfied:
-                conditions.satisfied.remove(key)
-        else:
-            conditions.satisfied.add(key)
-        conditions.update_conditions()
-    return callback
-
-
-def random_file(path_to_file_folder):
-    a=random.choice(os.listdir(path_to_file_folder))
-    while (a=='template')|(a=='.ipynb_checkpoints')|(not os.path.isdir(os.path.join(path_to_file_folder,a))):
-        a=random.choice(os.listdir(path_to_file_folder))
-    path_to_file = os.path.join(path_to_file_folder, a+'/')
-    b = random.choice(os.listdir(path_to_file))
-    while (b=='.ipynb_checkpoints'):
-        b=random.choice(os.listdir(path_to_file))
-    path_to_file = os.path.join(path_to_file, b)
-    return path_to_file
-
-
-def set_state_variables(d, headless=False):
-    if not headless:
-        factory = tk.IntVar
-    else:
-        factory = PseudoIntVar
-
-    for k, v in d.items():
-        if isinstance(v, dict):
-            set_state_variables(v, headless)
-        if isinstance(v, (int, float)):
-            d[k] = factory(value=v)
-        # if isinstance(v, str):
-        #     d[k] = tk.StringVar(value=v)
-
-
-class PseudoIntVar:
-    def __init__(self, value):
-        self.value = value
-
-    def get(self):
-        return self.value
-
-    def set(self, value):
-        self.value = value
-
-
-def pythonize_state_dict(d=None):
-    out = {}
-    if d is None:
-        d = state
-    for k, v in d.items():
-        if isinstance(v, dict):
-            out[k] = pythonize_state_dict(v)
-        elif hasattr(v, 'get'):
-            out[k] = v.get()
-        else:
-            out[k] = v
-    return out
-
-
-@conditions.satisfies('input')
-def get_image_dirname(label):
-    fname = askdirectory(title='Raw image directory')
-    if fname:
-        state['paths']['input'] = fname
-        set_label('input', label, fname)
-    return fname
-
-
-def read_template_file(fname, label):
-    state['template'] = cv.imdecode(np.fromfile(fname, dtype=np.uint8), cv.IMREAD_GRAYSCALE)
-    # IMREAD_GRAYSCALE has 0 enum of imread modes
-    set_label('template', label, fname)
-
-
-@conditions.satisfies('template')
-def get_template_file(label):
-    fname = askopenfilename(title='Seed template file')
-    if fname:
-        state['paths']['template_file'] = fname
-        read_template_file(fname, label)
-    return fname
-
-
-def get_out_dirname(label):
-    fname = askdirectory(title='Output directory')
-    if fname:
-        state['paths']['out_dir'] = fname
-        set_label('outdir', label, fname)
-    return fname
-
-
-def blur(img_widget, event):
-    morph = state['settings']['morph'].get()
-    gauss = state['settings']['gauss'].get()
-    canny_bottom = 0
-    canny_top = state['settings']['canny_top'].get()
-
-    src = state['img_arr'].copy()
-
-    bl = cv.GaussianBlur(src, (gauss, gauss), 0)
-    kernel = cv.getStructuringElement(cv.MORPH_ELLIPSE, (morph, morph))
-    closed = cv.morphologyEx(bl, cv.MORPH_CLOSE, kernel)
-    canny = cv.Canny(closed, canny_bottom, canny_top)
-    closed = cv.morphologyEx(canny, cv.MORPH_CLOSE, kernel)
-    contours0 = cv.findContours(closed, cv.RETR_EXTERNAL, cv.CHAIN_APPROX_SIMPLE)[0]
-    (contours0, _) = contours.sort_contours(contours0)
-    real_conts = []
-    src = cv.cvtColor(src, cv.COLOR_BGR2RGB)
-
-    for cont in contours0:
-        center, radius = cv.minEnclosingCircle(cont)
-        if ((cv.contourArea(cont) > CONTOUR_AREA_THRESHOLD) and
-                (center[0] > src.shape[1] // 4) & (center[0] < 2 * src.shape[1] // 3)):
-            cv.drawContours(src, [cont], -1, (255, 0, 0), -2)
-            real_conts.append(cont)
-
-    src = src.astype('uint8')
-    src = imutils.resize(src, height=500)
-    obj = ImageTk.PhotoImage(Image.fromarray(src))
-    img_widget.image = obj
-    img_widget['image'] = obj
-
-
-def color(img_widget, hsv, event):
-
-    h1 = state['color']['h_bottom'].get()
-    s1 = state['color']['s_bottom'].get()
-    v1 = state['color']['v_bottom'].get()
-    h2 = state['color']['h_top'].get()
-    s2 = state['color']['s_top'].get()
-    v2 = state['color']['v_top'].get()
-
-    # формируем начальный и конечный цвет фильтра
-    h_min = np.array((h1, s1, v1), np.uint8)
-    h_max = np.array((h2, s2, v2), np.uint8)
-
-    # накладываем фильтр на кадр в модели HSV
-    thresh = cv.inRange(hsv, h_min, h_max)
-
-    thresh = thresh.astype('uint8')
-    thresh = imutils.resize(thresh, height=420)
-    obj_color = ImageTk.PhotoImage(Image.fromarray(thresh))
-    img_widget.image = obj_color
-    img_widget['image'] = obj_color
-
-
-def seed(img_widget, event):
-    h1 = state['seed']['h_bottom'].get()
-    s1 = state['seed']['s_bottom'].get()
-    v1 = state['seed']['v_bottom'].get()
-    h2 = state['seed']['h_top'].get()
-    s2 = state['seed']['s_top'].get()
-    v2 = state['seed']['v_top'].get()
-
-    h_min = np.array((h1, s1, v1), np.uint8)
-    h_max = np.array((h2, s2, v2), np.uint8)
-
-    src = state['img_arr'].copy()
-    hsv = cv.cvtColor(src, cv.COLOR_BGR2HSV)
-    thresh = cv.inRange(hsv, h_min, h_max)
-    thresh = thresh.astype('uint8')
-    thresh = imutils.resize(thresh, height=420)
-    obj_color = ImageTk.PhotoImage(Image.fromarray(thresh))
-    img_widget.image = obj_color
-    img_widget['image'] = obj_color
-
-
-def rotate_pic(img, rotate, resize=False):
-    rotate_dict = {
-        90: cv.ROTATE_90_CLOCKWISE,
-        180: cv.ROTATE_180,
-        270: cv.ROTATE_90_COUNTERCLOCKWISE}
-
-    if rotate:
-        img = cv.rotate(img, rotate_dict[rotate])
-    if resize:
-        img = imutils.resize(img, height=300)
-    return img
-
-
-def choose_rotation(angle, img, img_widget,label):
-    img = rotate_pic(img, angle, True)
-    i = ImageTk.PhotoImage(Image.fromarray(img))
-    img_widget.image = i
-    img_widget['image'] = i
-    set_label('rotation', label, state['rotation'])
-
-
-def rotation(w, label):
-    window = tk.Toplevel(w)
-    window.title('Rotate image')
-    window.geometry('600x400')
-    control_frame = tk.Frame(master=window)
-
-    text_lbl = tk.Label(control_frame, text='Choose the angle to rotate your photos, as in the example')
-    img_frame = tk.Frame(master=window)
-
-    path_to_ethalon = os.path.dirname(os.path.abspath(__file__))
-    ethalon = cv.imdecode(np.fromfile(os.path.join(path_to_ethalon, 'ethalon.png'), dtype=np.uint8), cv.IMREAD_COLOR)
-#     ethalon = cv.imread(os.path.join(path_to_ethalon, 'ethalon.png'))
-    ethalon = cv.cvtColor(ethalon, cv.COLOR_BGR2RGB)
-    ethalon = ethalon.astype('uint8')
-    ethalon = imutils.resize(ethalon, height=300)
-    obj = ImageTk.PhotoImage(Image.fromarray(ethalon))
-
-    test_img = cv.imdecode(np.fromfile(random_file(state['paths']['input']), dtype=np.uint8), cv.IMREAD_COLOR)
-#     test_img = cv.imread(random_file(state['paths']['input']))
-    test_img = cv.cvtColor(test_img, cv.COLOR_BGR2RGB)
-    test_img = test_img.astype('uint8')
-    test_img = imutils.resize(test_img, height=300)
-    obj2 = ImageTk.PhotoImage(Image.fromarray(test_img))
-
-    maxsize = max(test_img.shape[:2])
-    window.geometry(f'{maxsize * 2}x{maxsize + 100}')
-
-    img1 = tk.Label(master=img_frame, width=maxsize, height=maxsize)
-    img1.image = obj
-    img1['image'] = obj
-
-    img2 = tk.Label(master=img_frame, width=maxsize, height=maxsize)
-    img2.image = obj2
-    img2['image'] = obj2
-    choose_rotation(state['rotation'].get(), test_img, img2,label)
-
-    buttons = []
-    for i, val in enumerate([0, 90, 180, 270]):
-        buttons.append(tk.Radiobutton(control_frame, text=str(val), command=lambda j=val: choose_rotation(j, test_img, img2, label),
-                                      variable=state['rotation'], value=val))
-
-    set_button = tk.Button(window, text='Save', command=window.destroy)
-    img_frame.grid(column=0, row=0, sticky=tk.W + tk.E)
-    control_frame.grid(column=0, row=1)
-
-    img1.grid(column=0, row=0)
-    img2.grid(column=1, row=0)
-
-    text_lbl.grid(column=0, row=0, columnspan=4)
-    for i, b in enumerate(buttons):
-        b.grid(column=i, row=1)
-    set_button.grid(column=0, row=2, columnspan=4)
-    window.columnconfigure(0, weight=1)
-
-
-def clear(w): # clear all the wigets
-    for c in w.grid_slaves():
-        c.destroy()
-
-
-def set_params(parameter):
-    for i in state[parameter]:
-        state[parameter][i] = state['color'][i].get()
-
-
-def add_color_sliders(d, frame, command, startrow=1):
-    for i, param in enumerate('hsv'):
-        row = startrow + 2 * i
-        name = tk.Label(master=frame, text=param)
-        name.grid(column=0, row=row, rowspan=2)
-        for j, suffix in enumerate(['bottom', 'top']):
-            var = d[f'{param}_{suffix}']
-            label = tk.Label(master=frame, textvariable=var)
-            slider = tk.Scale(master=frame, from_=0, to=255, variable=var, orient='horizontal', resolution=1, showvalue=False, command=command)
-            slider.grid(column=j + 1, row=row)
-            label.grid(column=j + 1, row=row + 1)
-    return row + 1
-
-
-def seeds_tab(img, tweak_frame):
-    clear(tweak_frame)
-    seed(img, None)
-
-    color_label = tk.Label(master=tweak_frame, text="Choosing color for seed excluding")
-    color_label.grid(column=0, row=0, columnspan=3)
-    row = 1 + add_color_sliders(state['seed'], tweak_frame, partial(seed, img))
-    button_b2 = tk.Button(tweak_frame, text='Back', command=partial(colors_tab, img, tweak_frame))
-    button_end = tk.Button(tweak_frame, text='Done', command=tweak_frame.winfo_toplevel().destroy)
-    button_b2.grid(column=0, row=row)
-    button_end.grid(column=2, row=row)
-
-
-def colors_tab(img, tweak_frame):
-    src = state['img_arr'].copy()
-    template = state['template']
-    template = rotate_pic(template, state['rotation'].get())
-    w, h = template.shape[::-1]
-
-    method = cv.TM_CCOEFF_NORMED
-    res = cv.matchTemplate(state['img_arr_0'], template, method)
-    threshold = 0.55
-    loc = np.where(res > threshold)
-    numbers0 = []
-    for pt in zip(*loc[::-1]):
-        if (pt[0] > src.shape[1] / 3) and (pt[0] < 2 * src.shape[1] / 3):
-            numbers0.append(pt[0])
-
-    numbers = pd.Series(numbers0)
-    mode = numbers.mode()[0]
-    mean_left_x = int(mode) - w // 4
-    mean_right_x = int(mode) + 3 * w // 4
-    mean_left_x = round(mean_left_x)
-    mean_right_x = round(mean_right_x)
-
-    overlay = src.copy()
-    cv.rectangle(overlay, (0, src.shape[0]), (mean_left_x, 0), (0,224,79), -1)
-    opacity = 0.25
-    cv.rectangle(overlay, (mean_right_x, src.shape[0]), (src.shape[1], 0), (240, 0, 255), -5)
-    cv.addWeighted(overlay, opacity, src, 1 - opacity, 0, src)
-    hsv = cv.cvtColor(src, cv.COLOR_BGR2HSV)
-
-    clear(tweak_frame)
-    color(img, hsv, None)
-
-    color_label = tk.Label(master=tweak_frame, text="Choosing color for pixel counting")
-    color_label.grid(column=0, row=0, columnspan=3)
-    row = add_color_sliders(state['color'], tweak_frame, partial(color, img, hsv)) + 1
-
-    button_b1 = tk.Button(tweak_frame, text='Set sprouts', command=partial(set_params, 'leaves'))
-    button_n2 = tk.Button(tweak_frame, text='Set roots', command=partial(set_params, 'roots'))
-    button_b1.grid(column=0, row=row)
-    button_n2.grid(column=2, row=row)
-    button_b1 = tk.Button(tweak_frame, text='Back', command=partial(contours_tab, img, tweak_frame))
-    button_n2 = tk.Button(tweak_frame, text='Next', command=partial(seeds_tab, img, tweak_frame))
-    button_b1.grid(column=0, row=row+1)
-    button_n2.grid(column=2, row=row+1)
-
-
-def contours_tab(img, tweak_frame):
-    clear(tweak_frame)
-    blur(img, None)
-
-    morph_label = tk.Label(master=tweak_frame, text="Choosing parameters for contour recognition")
-    morph_label.grid(column=0, row=0, columnspan=3)
-    morph_slider_lbl = tk.Label(master=tweak_frame, textvariable=state['settings']['morph'])
-    morph_name_lbl = tk.Label(master=tweak_frame, text="morph:")
-    morph_slider = tk.Scale(master=tweak_frame, from_=1, to=13, resolution=2, orient='horizontal', showvalue=False, command=partial(blur, img),
-                             variable=state['settings']['morph'])
-    morph_name_lbl.grid(column=0, row=1)
-    morph_slider.grid(column=1, row=1)
-    morph_slider_lbl.grid(column=2, row=1)
-
-    gauss_slider_lbl = tk.Label(master=tweak_frame, textvariable=state['settings']['gauss'])
-    gauss_name_lbl = tk.Label(master=tweak_frame, text='gauss:')
-    gauss_slider = tk.Scale(master=tweak_frame, from_=1, to=13, resolution=2, orient='horizontal', showvalue=False, command=partial(blur, img),
-                             variable=state['settings']['gauss'])
-    gauss_name_lbl.grid(column=0, row=2)
-    gauss_slider.grid(column=1, row=2)
-    gauss_slider_lbl.grid(column=2, row=2)
-
-    canny_top_slider_lbl = tk.Label(master=tweak_frame, textvariable=state['settings']['canny_top'])
-    canny_top_name_lbl = tk.Label(master=tweak_frame, text='canny_top:')
-    canny_top_slider = tk.Scale(master=tweak_frame, from_=0, to=255, orient='horizontal', showvalue=False, command=partial(blur, img),
-                                 variable=state['settings']['canny_top'])
-    canny_top_name_lbl.grid(column=0, row=3)
-    canny_top_slider.grid(column=1, row=3)
-    canny_top_slider_lbl.grid(column=2, row=3)
-
-    button_n1 = tk.Button(tweak_frame, text='Next', command=partial(colors_tab, img, tweak_frame))
-    button_n1.grid(column=2, row=4)
-
-
-def tweak_image(w):
-    window = tk.Toplevel(w)
-    window.title('Tweak image')
-    window.geometry('900x650')
-
-    file_name = random_file(state['paths']['input'])
-    img_arr = cv.imdecode(np.fromfile(file_name, dtype=np.uint8), cv.IMREAD_COLOR) ## IMREAD_UNCHANGED has -1 enum of imread modes
-    img_arr = rotate_pic(img_arr, state['rotation'].get())
-    img_arr_0 = cv.imdecode(np.fromfile(file_name, dtype=np.uint8), cv.IMREAD_GRAYSCALE)## IMREAD_GRAYSCALE has 0 enum of imread modes
-    img_arr_0 = rotate_pic(img_arr_0, state['rotation'].get())
-    state['img_arr'] = img_arr
-    state['img_arr_0'] = img_arr_0
-
-    img_frame = tk.Frame(master=window)
-    img = tk.Label(master=img_frame)
-    img.pack(fill=tk.BOTH, expand=True)
-    img_frame.pack()
-    tweak_frame = tk.Frame(master=window)
-    tweak_frame.pack()
-
-    contours_tab(img, tweak_frame)
+import tkinter as tk
+from tkinter.filedialog import askopenfilename, askdirectory, asksaveasfilename
+from PIL import ImageTk, Image
+import cv2 as cv
+import imutils
+from imutils import contours
+import numpy as np
+import pandas as pd
+import os
+import random
+from functools import partial
+import json
+import logging
+from scipy import stats
+
+
+state = {
+    'settings': {
+        'morph': 5,
+        'gauss': 3,
+        'canny_top': 160
+    },
+    'roots': {
+        'h_bottom': 50,
+        'h_top': 255,
+        's_bottom': 0,
+        's_top': 255,
+        'v_bottom': 100,
+        'v_top': 255,
+    },
+    'leaves': {
+        'h_bottom': 0,
+        'h_top': 50,
+        's_bottom': 0,
+        's_top': 255,
+        'v_bottom': 100,
+        'v_top': 255,
+    },
+    'seed': {
+        'h_bottom': 0,
+        'h_top': 20,
+        's_bottom': 100,
+        's_top': 255,
+        'v_bottom': 100,
+        'v_top': 255,
+    },
+    'paths': {
+        'out_dir': os.getcwd()
+    },
+    'rotation': 0,
+    'paper_area_thresold': 1000,
+    'paper_area': 0,
+    'germ_thresh': 10,
+    'progress': 0,
+    'is_seed_big':0
+}
+
+STATE_SYNTAX_VERSION = 2
+STATE_SYNTAX_VERSION_KEY = 'syntax_version'
+CONTOUR_AREA_THRESHOLD = 1000  
+FORMAT='{:.0f}'
+
+class FormatLabel(tk.Label):
+
+    def __init__(self, master=None, cnf={}, **kw):
+
+        # default values
+        self._format = FORMAT
+        self._textvariable = None
+        self.two_n_plus1 = None
+
+        # get new format and remove it from `kw` so later `super().__init__` doesn't use them (it would get error message)
+        if 'format' in kw:
+            self._format = kw['format']
+            del kw['format']
+
+        # get `textvariable` to assign own function which set formatted text in Label when variable change value
+        if 'textvariable' in kw:
+            self._textvariable = kw['textvariable']
+            self._trace_id = self._textvariable.trace('w', self._update_text)
+            del kw['textvariable']
+
+        # run `Label.__init__` without `format` and `textvariable`
+        super().__init__(master, cnf={}, **kw)
+
+        # update text after running `Label.__init__`
+        if self._textvariable:
+            #self._update_text(None, None, None)
+            self._update_text(self._textvariable, '', 'w')
+
+    def _update_text(self, a, b, c):
+        """update text in label when variable change value"""
+        self["text"] = self._format.format(self._textvariable.get())
+
+    def destroy(self):
+        self._textvariable.trace_vdelete('w', self._trace_id)
+        super().destroy()
+
+
+class LoggingToGUI(logging.Handler):
+    # https://stackoverflow.com/a/18194597/1258041
+    def __init__(self, console):
+        logging.Handler.__init__(self)
+        self.console = console
+
+    def emit(self, message):
+        formattedMessage = self.format(message)
+
+        self.console.configure(state=tk.NORMAL)
+        self.console.insert(tk.END, formattedMessage + '\n')
+        self.console.configure(state=tk.DISABLED)
+        self.console.see(tk.END)
+
+
+def save_state(fname):
+    state_dict = pythonize_state_dict()
+    for k in ['template', 'img_arr', 'img_arr_0', 'progress', 'abort_flag']:
+        state_dict.pop(k, None)
+    state_dict[STATE_SYNTAX_VERSION_KEY] = STATE_SYNTAX_VERSION
+    with open(fname, 'w') as f:
+        json.dump(state_dict, f)
+
+
+def update_dict(old, new):
+    for k, v in new.items():
+        if isinstance(v, dict):
+            update_dict(old[k], v)
+        elif k in old and hasattr(old[k], 'set'):
+            old[k].set(v)
+        else:
+            old[k] = v
+
+
+def load_state(fname, label_dict):
+    with open(fname) as f:
+        d = json.load(f)
+    if d[STATE_SYNTAX_VERSION_KEY] == 1:
+        d.pop('color', None)
+    update_dict(state, d)
+    set_state_variables(state)
+    update_labels(label_dict)
+    conditions.check_conditions()
+    conditions.update_conditions()
+
+
+def load_state_headless(fname):
+    set_state_variables(state, headless=True)
+    with open(fname) as f:
+        d = json.load(f)
+    update_dict(state, d)
+
+
+def update_labels(label_dict):
+    inp = state.get('paths', {}).get('input')
+    if inp:
+        set_label('input', label_dict['input'], inp)
+
+    template = state.get('paths', {}).get('template_file')
+    if template:
+        read_template_file(template, label_dict['template'])
+
+    outdir = state.get('paths', {}).get('out_dir')
+    if outdir:
+        set_label('outdir', label_dict['outdir'], outdir)
+
+    rotate = state.get('rotation')
+    if rotate:
+        set_label('rotation', label_dict['rotation'], rotate)
+
+
+def set_label(kind, label, value):
+    mapping = {
+        'input': lambda fname: f'Selected image directory: {os.path.basename(fname)}.',
+        'template': lambda fname: f'Selected seed template: {os.path.basename(fname)}.',
+        'outdir': lambda fname: f'Output directory: {os.path.basename(fname)}.',
+        'rotation': lambda angle: f'Rotation angle: {angle.get()}.'
+    }
+    label['text'] = mapping[kind](value)
+
+
+def load_state_dialog(label_dict):
+    fname = askopenfilename(title="Load settings...", filetypes=[('JSON files', '*.json'), ('All files', '*')])
+    if fname:
+        load_state(fname, label_dict)
+
+
+def save_state_dialog():
+    fname = asksaveasfilename(title="Save settings as...", defaultextension='.json')
+    if fname:
+        save_state(fname)
+
+
+class ConditionManager:
+    CONDITIONS = {
+        'rotate': ['input'],
+        'tweak': ['input', 'template'],
+        'run': ['input', 'template', 'paper_area', 'germ_thresh']
+    }
+    def __init__(self):
+        self.satisfied = set()
+
+    def register(self, widgets):
+        self.widgets = widgets
+        for k, w in widgets.items():
+            if k in self.CONDITIONS:
+                for widget in w:
+                    widget['state'] = tk.DISABLED
+
+    def satisfies(self, condition):
+        """Decorator that makes a function call satisfy the corresponding condition.
+        Changes the status of widgets after a successful call."""
+        def decorator(func):
+            def wrapped(*args, **kwargs):
+                ret = func(*args, **kwargs)
+                if ret:
+                    self.satisfied.add(condition)
+                    self.update_conditions()
+                return ret
+            return wrapped
+        return decorator
+
+    def update_conditions(self):
+        for key, v in self.CONDITIONS.items():
+            if all(w in self.satisfied for w in v) and key in self.widgets:
+                status = tk.NORMAL
+            else:
+                status = tk.DISABLED
+            for w in self.widgets[key]:
+                w['state'] = status
+
+    def check_conditions(self):
+        if state.get('paths', {}).get('input'):
+            self.satisfied.add('input')
+        if state.get('paths', {}).get('template_file'):
+            self.satisfied.add('template')
+        if state.get('paper_area').get():
+            self.satisfied.add('paper_area')
+        if state.get('germ_thresh').get():
+            self.satisfied.add('germ_thresh')
+
+
+conditions = ConditionManager()
+
+
+def trace_entry(key):
+    def callback(name, index, op):
+        try:
+            assert state[key].get() != 0
+        except (AssertionError, tk.TclError):
+            if key in conditions.satisfied:
+                conditions.satisfied.remove(key)
+        else:
+            conditions.satisfied.add(key)
+        conditions.update_conditions()
+    return callback
+
+
+
+def random_file(path_to_file_folder):
+    a=random.choice(os.listdir(path_to_file_folder))
+    not_needed_folders_list = ['.ipynb_checkpoints', 'template', 'color_block_separation', 'seeds_search', 'contours']
+    while any(a==i for i in not_needed_folders_list)|(not os.path.isdir(os.path.join(path_to_file_folder,a))):
+        a=random.choice(os.listdir(path_to_file_folder))
+    path_to_file = os.path.join(path_to_file_folder, a+'/')
+    b = random.choice(os.listdir(path_to_file))
+    while any(b==i for i in not_needed_folders_list):
+        b=random.choice(os.listdir(path_to_file))
+    path_to_file = os.path.join(path_to_file, b)
+    return path_to_file
+
+
+def set_state_variables(d, headless=False):
+    if not headless:
+        factory = tk.IntVar
+    else:
+        factory = PseudoIntVar
+
+    for k, v in d.items():
+        if isinstance(v, dict):
+            set_state_variables(v, headless)
+        if isinstance(v, (int, float)):
+            d[k] = factory(value=v)
+        # if isinstance(v, str):
+        #     d[k] = tk.StringVar(value=v)
+
+
+class PseudoIntVar:
+    def __init__(self, value):
+        self.value = value
+
+    def get(self):
+        return self.value
+
+    def set(self, value):
+        self.value = value
+
+
+def pythonize_state_dict(d=None):
+    out = {}
+    if d is None:
+        d = state
+    for k, v in d.items():
+        if isinstance(v, dict):
+            out[k] = pythonize_state_dict(v)
+        elif hasattr(v, 'get'):
+            out[k] = v.get()
+        else:
+            out[k] = v
+    return out
+
+
+@conditions.satisfies('input')
+def get_image_dirname(label):
+    fname = askdirectory(title='Raw image directory')
+    if fname:
+        state['paths']['input'] = fname
+        set_label('input', label, fname)
+    return fname
+
+
+def read_template_file(fname, label):
+    state['template'] = cv.imdecode(np.fromfile(fname, dtype=np.uint8), cv.IMREAD_GRAYSCALE)
+    # IMREAD_GRAYSCALE has 0 enum of imread modes
+    set_label('template', label, fname)
+
+
+@conditions.satisfies('template')
+def get_template_file(label):
+    fname = askopenfilename(title='Seed template file')
+    if fname:
+        state['paths']['template_file'] = fname
+        read_template_file(fname, label)   
+    return fname
+
+
+def get_out_dirname(label):
+    fname = askdirectory(title='Output directory')
+    if fname:
+        state['paths']['out_dir'] = fname
+        set_label('outdir', label, fname)
+    return fname
+
+
+def blur(img_widget, event):
+    morph = state['settings']['morph'].get()
+    gauss = state['settings']['gauss'].get()
+    canny_bottom = 0
+    canny_top = state['settings']['canny_top'].get()
+
+    src = state['img_arr'].copy()
+
+    bl = cv.GaussianBlur(src, (gauss, gauss), 0)
+    kernel = cv.getStructuringElement(cv.MORPH_ELLIPSE, (morph, morph))
+    closed = cv.morphologyEx(bl, cv.MORPH_CLOSE, kernel)
+    canny = cv.Canny(closed, canny_bottom, canny_top)
+    closed = cv.morphologyEx(canny, cv.MORPH_CLOSE, kernel)
+    contours0 = cv.findContours(closed, cv.RETR_EXTERNAL, cv.CHAIN_APPROX_SIMPLE)[0]
+    (contours0, _) = contours.sort_contours(contours0)
+    real_conts = []
+    src = cv.cvtColor(src, cv.COLOR_BGR2RGB)
+
+    for cont in contours0:
+        center, radius = cv.minEnclosingCircle(cont)
+        if ((cv.contourArea(cont) > CONTOUR_AREA_THRESHOLD) and
+                (center[0] > src.shape[1] // 4) & (center[0] < 2 * src.shape[1] // 3)):
+            cv.drawContours(src, [cont], -1, (255, 0, 0), -2)
+            real_conts.append(cont)
+
+    src = src.astype('uint8')
+    src = imutils.resize(src, height=500)
+    obj = ImageTk.PhotoImage(Image.fromarray(src))
+    img_widget.image = obj
+    img_widget['image'] = obj
+
+
+def color(img_widget, hsv, obj, event):
+
+    h1 = state[obj]['h_bottom'].get()
+    s1 = state[obj]['s_bottom'].get()
+    v1 = state[obj]['v_bottom'].get()
+    h2 = state[obj]['h_top'].get()
+    s2 = state[obj]['s_top'].get()
+    v2 = state[obj]['v_top'].get()
+
+    # формируем начальный и конечный цвет фильтра
+    h_min = np.array((h1, s1, v1), np.uint8)
+    h_max = np.array((h2, s2, v2), np.uint8)
+
+    # накладываем фильтр на кадр в модели HSV
+    thresh = cv.inRange(hsv, h_min, h_max)
+
+    thresh = thresh.astype('uint8')
+    thresh = imutils.resize(thresh, height=420)
+    obj_color = ImageTk.PhotoImage(Image.fromarray(thresh))
+    img_widget.image = obj_color
+    img_widget['image'] = obj_color
+
+
+def seed(img_widget, event):
+    h1 = state['seed']['h_bottom'].get()
+    s1 = state['seed']['s_bottom'].get()
+    v1 = state['seed']['v_bottom'].get()
+    h2 = state['seed']['h_top'].get()
+    s2 = state['seed']['s_top'].get()
+    v2 = state['seed']['v_top'].get()
+
+    h_min = np.array((h1, s1, v1), np.uint8)
+    h_max = np.array((h2, s2, v2), np.uint8)
+
+    src = state['img_arr'].copy()
+    hsv = cv.cvtColor(src, cv.COLOR_BGR2HSV)
+    thresh = cv.inRange(hsv, h_min, h_max)
+    thresh = thresh.astype('uint8')
+    thresh = imutils.resize(thresh, height=420)
+    obj_color = ImageTk.PhotoImage(Image.fromarray(thresh))
+    img_widget.image = obj_color
+    img_widget['image'] = obj_color
+
+
+def rotate_pic(img, rotate, resize=False):
+    rotate_dict = {
+        90: cv.ROTATE_90_CLOCKWISE,
+        180: cv.ROTATE_180,
+        270: cv.ROTATE_90_COUNTERCLOCKWISE}
+
+    if rotate:
+        img = cv.rotate(img, rotate_dict[rotate])
+    if resize:
+        img = imutils.resize(img, height=300)
+    return img
+
+
+def choose_rotation(angle, img, img_widget,label):
+    img = rotate_pic(img, angle, True)
+    i = ImageTk.PhotoImage(Image.fromarray(img))
+    img_widget.image = i
+    img_widget['image'] = i
+    set_label('rotation', label, state['rotation'])
+
+
+def rotation(w, label):
+    window = tk.Toplevel(w)
+    window.title('Rotate image')
+    window.geometry('600x400')
+    control_frame = tk.Frame(master=window)
+
+    text_lbl = tk.Label(control_frame, text='Choose the angle to rotate your photos, as in the example')
+    img_frame = tk.Frame(master=window)
+
+    path_to_ethalon = os.path.dirname(os.path.abspath(__file__))
+    ethalon = cv.imdecode(np.fromfile(os.path.join(path_to_ethalon, 'ethalon.png'), dtype=np.uint8), cv.IMREAD_COLOR)
+#     ethalon = cv.imread(os.path.join(path_to_ethalon, 'ethalon.png'))
+    ethalon = cv.cvtColor(ethalon, cv.COLOR_BGR2RGB)
+    ethalon = ethalon.astype('uint8')
+    ethalon = imutils.resize(ethalon, height=300)
+    obj = ImageTk.PhotoImage(Image.fromarray(ethalon))
+
+    test_img = cv.imdecode(np.fromfile(random_file(state['paths']['input']), dtype=np.uint8), cv.IMREAD_COLOR)
+#     test_img = cv.imread(random_file(state['paths']['input']))
+    test_img = cv.cvtColor(test_img, cv.COLOR_BGR2RGB)
+    test_img = test_img.astype('uint8')
+    test_img = imutils.resize(test_img, height=300)
+    obj2 = ImageTk.PhotoImage(Image.fromarray(test_img))
+
+    maxsize = max(test_img.shape[:2])
+    window.geometry(f'{maxsize * 2}x{maxsize + 100}')
+
+    img1 = tk.Label(master=img_frame, width=maxsize, height=maxsize)
+    img1.image = obj
+    img1['image'] = obj
+
+    img2 = tk.Label(master=img_frame, width=maxsize, height=maxsize)
+    img2.image = obj2
+    img2['image'] = obj2
+    choose_rotation(state['rotation'].get(), test_img, img2,label)
+
+    buttons = []
+    for i, val in enumerate([0, 90, 180, 270]):
+        buttons.append(tk.Radiobutton(control_frame, text=str(val), command=lambda j=val: choose_rotation(j, test_img, img2, label),
+                                      variable=state['rotation'], value=val))
+
+    set_button = tk.Button(window, text='Save', command=window.destroy)
+    img_frame.grid(column=0, row=0, sticky=tk.W + tk.E)
+    control_frame.grid(column=0, row=1)
+
+    img1.grid(column=0, row=0)
+    img2.grid(column=1, row=0)
+
+    text_lbl.grid(column=0, row=0, columnspan=4)
+    for i, b in enumerate(buttons):
+        b.grid(column=i, row=1)
+    set_button.grid(column=0, row=2, columnspan=4)
+    window.columnconfigure(0, weight=1)
+
+
+def clear(w): # clear all the wigets
+    for c in w.grid_slaves():
+        c.destroy()
+
+
+# def set_params(parameter):
+#     for i in state[parameter]:
+#         state[parameter][i] = state['color'][i].get()
+
+
+def add_color_sliders(d, frame, command, startrow=1):
+    for i, param in enumerate('hsv'):
+        row = startrow + 2 * i
+        name = tk.Label(master=frame, text=param)
+        name.grid(column=0, row=row, rowspan=2)
+        for j, suffix in enumerate(['bottom', 'top']):
+            var = d[f'{param}_{suffix}']
+            label = tk.Label(master=frame, textvariable=var)
+            slider = tk.Scale(master=frame, from_=0, to=255, variable=var, orient='horizontal', resolution=1, showvalue=False, command=command)
+            slider.grid(column=j + 1, row=row)
+            label.grid(column=j + 1, row=row + 1)
+    return row + 1
+
+
+def seeds_tab(img, tweak_frame):
+    tweak_frame.winfo_toplevel().title('Recognition settings: seeds')
+    clear(tweak_frame)
+    seed(img, None)
+
+    color_label = tk.Label(master=tweak_frame, text="Choose color range for seed exclusion")
+    color_label.grid(column=0, row=0, columnspan=3)
+    row = 1 + add_color_sliders(state['seed'], tweak_frame, partial(seed, img))
+    button_b2 = tk.Button(tweak_frame, text='Back', command=partial(colors_tab, img, tweak_frame, 'roots'))
+    button_end = tk.Button(tweak_frame, text='Done', command=tweak_frame.winfo_toplevel().destroy)
+    button_b2.grid(column=0, row=row)
+    button_end.grid(column=2, row=row)
+
+
+def colors_tab(img, tweak_frame, obj):
+    import matplotlib
+    from matplotlib import pyplot as plt
+    src = state['img_arr'].copy()
+    template = state['template']
+    template = rotate_pic(template, state['rotation'].get())
+    w, h = template.shape[::-1]
+
+    method = cv.TM_CCOEFF_NORMED
+    res = cv.matchTemplate(state['img_arr_0'], template, method)
+    threshold = 0.55
+    loc = np.where(res > threshold)
+    numbers0 = []
+    for pt in zip(*loc[::-1]):
+        if (pt[0] > src.shape[1] / 3) and (pt[0] < 2 * src.shape[1] / 3):
+            numbers0.append(pt[0])
+
+    numbers = pd.Series(numbers0)
+    mode = numbers.mode()[0]
+    mean_left_x = int(mode) - w // 4
+    mean_right_x = int(mode) + 3 * w // 4
+    mean_left_x = round(mean_left_x)
+    mean_right_x = round(mean_right_x)
+
+    overlay = src.copy()
+    cv.rectangle(overlay, (0, src.shape[0]), (mean_left_x, 0), (0,224,79), -1)
+    opacity = 0.25
+    cv.rectangle(overlay, (mean_right_x, src.shape[0]), (src.shape[1], 0), (240, 0, 255), -5)
+    cv.addWeighted(overlay, opacity, src, 1 - opacity, 0, src)
+    hsv = cv.cvtColor(src, cv.COLOR_BGR2HSV)
+
+    tweak_frame.winfo_toplevel().title('Recognition settings: ' + obj)
+    clear(tweak_frame)
+    color(img, hsv, obj, None)
+
+    color_label = tk.Label(master=tweak_frame, text=f"Choose color range for {obj} detection.")
+    color_label.grid(column=0, row=0, columnspan=3)
+    row = add_color_sliders(state[obj], tweak_frame, partial(color, img, hsv, obj)) + 1
+
+    # button_b1 = tk.Button(tweak_frame, text='Set sprouts', command=partial(set_params, 'leaves'))
+    # button_n2 = tk.Button(tweak_frame, text='Set roots', command=partial(set_params, 'roots'))
+    # button_b1.grid(column=0, row=row)
+    # button_n2.grid(column=2, row=row)
+    if obj == 'leaves':
+        back_command = partial(contours_tab, img, tweak_frame)
+        next_command = partial(colors_tab, img, tweak_frame, 'roots')
+    elif obj == 'roots':
+        back_command = partial(colors_tab, img, tweak_frame, 'leaves')
+        next_command = partial(seeds_tab, img, tweak_frame)
+    else:
+        raise ValueError(f'Unsupported value for `obj`: {obj}. Must be "leaves" or "roots".')
+    button_b1 = tk.Button(tweak_frame, text='Back', command=back_command)
+    button_n2 = tk.Button(tweak_frame, text='Next', command=next_command)
+    button_b1.grid(column=0, row=row+1)
+    button_n2.grid(column=2, row=row+1)
+
+
+def contours_tab(img, tweak_frame):
+    clear(tweak_frame)
+    blur(img, None)
+
+    morph_label = tk.Label(master=tweak_frame, text="Choosing parameters for contour recognition")
+    morph_label.grid(column=0, row=0, columnspan=3)
+    morph_slider_lbl = tk.Label(master=tweak_frame, textvariable=state['settings']['morph'])
+    morph_name_lbl = tk.Label(master=tweak_frame, text="morph:")
+    morph_slider = tk.Scale(master=tweak_frame, from_=1, to=13, resolution=2, orient='horizontal', showvalue=False, command=partial(blur, img),
+                             variable=state['settings']['morph'])
+    morph_name_lbl.grid(column=0, row=1)
+    morph_slider.grid(column=1, row=1)
+    morph_slider_lbl.grid(column=2, row=1)
+
+    gauss_slider_lbl = tk.Label(master=tweak_frame, textvariable=state['settings']['gauss'])
+    gauss_name_lbl = tk.Label(master=tweak_frame, text='gauss:')
+    gauss_slider = tk.Scale(master=tweak_frame, from_=1, to=13, resolution=2, orient='horizontal', showvalue=False, command=partial(blur, img),
+                             variable=state['settings']['gauss'])
+    gauss_name_lbl.grid(column=0, row=2)
+    gauss_slider.grid(column=1, row=2)
+    gauss_slider_lbl.grid(column=2, row=2)
+
+    canny_top_slider_lbl = tk.Label(master=tweak_frame, textvariable=state['settings']['canny_top'])
+    canny_top_name_lbl = tk.Label(master=tweak_frame, text='canny_top:')
+    canny_top_slider = tk.Scale(master=tweak_frame, from_=0, to=255, orient='horizontal', showvalue=False, command=partial(blur, img),
+                                 variable=state['settings']['canny_top'])
+    canny_top_name_lbl.grid(column=0, row=3)
+    canny_top_slider.grid(column=1, row=3)
+    canny_top_slider_lbl.grid(column=2, row=3)
+
+    button_n1 = tk.Button(tweak_frame, text='Next', command=partial(colors_tab, img, tweak_frame, 'leaves'))
+    button_n1.grid(column=2, row=4)
+
+
+def tweak_image(w):
+    window = tk.Toplevel(w)
+    window.title('Tweak image')
+    window.geometry('900x650')        
+
+    template = cv.imdecode(np.fromfile(state['paths']['template_file'] , dtype=np.uint8), cv.IMREAD_COLOR) 
+    bl_t=cv.GaussianBlur(template,(5,5),0)
+    canny_t = cv.Canny(bl_t, 0, 140)
+    kernel_t = cv.getStructuringElement(cv.MORPH_ELLIPSE, (7,7))
+    closed_t = cv.morphologyEx(canny_t, cv.MORPH_CLOSE, kernel_t)
+    contours0_t = cv.findContours(closed_t.copy(), cv.RETR_EXTERNAL, cv.CHAIN_APPROX_SIMPLE)[0]
+    contour_area_threshold_index = np.array([cv.contourArea(cont) for cont in contours0_t]).argmax()
+    global CONTOUR_AREA_THRESHOLD
+    CONTOUR_AREA_THRESHOLD = cv.contourArea(contours0_t[contour_area_threshold_index])
+
+    file_name = random_file(state['paths']['input'])
+    img_arr = cv.imdecode(np.fromfile(file_name, dtype=np.uint8), cv.IMREAD_COLOR) ## IMREAD_UNCHANGED has -1 enum of imread modes
+    img_arr = rotate_pic(img_arr, state['rotation'].get())
+    img_arr_0 = cv.imdecode(np.fromfile(file_name, dtype=np.uint8), cv.IMREAD_GRAYSCALE)## IMREAD_GRAYSCALE has 0 enum of imread modes
+    img_arr_0 = rotate_pic(img_arr_0, state['rotation'].get())
+    state['img_arr'] = img_arr
+    state['img_arr_0'] = img_arr_0
+
+    img_frame = tk.Frame(master=window)
+    img = tk.Label(master=img_frame)
+    img.pack(fill=tk.BOTH, expand=True)
+    img_frame.pack()
+    tweak_frame = tk.Frame(master=window)
+    tweak_frame.pack()
+
+    contours_tab(img, tweak_frame)
```

### Comparing `morley-0.0.4/morley/logo.png` & `morley-0.0.5/morley/logo.png`

 * *Files identical despite different names*

### Comparing `morley-0.0.4/morley/main.py` & `morley-0.0.5/morley/main.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,195 +1,235 @@
-import tkinter as tk
-from tkinter import ttk
-import tkinter.scrolledtext as st
-import logging
-from functools import partial
-import os
-import sys
-import threading
-import argparse
-from . import gui, Morley, version
-
-logger = logging.getLogger()
-
-
-def start_gui():
-    window = tk.Tk()
-    path_to_icon = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'logo.png')
-    window.tk.call('wm', 'iconphoto', window._w, tk.PhotoImage(file=path_to_icon))
-    # Add image file
-    background_image = tk.PhotoImage(path_to_icon)
-    background_label = tk.Label(window, image=background_image)
-    background_label.place(x=0, y=0, relwidth=1, relheight=1)
-    background_label.image = background_image
-
-    window.title(f'Morley GUI v{version.version}')
-    window.geometry('960x430')
-
-    gui.set_state_variables(gui.state)
-
-    # https://stackoverflow.com/a/54068050/1258041
-    try:
-        try:
-            window.tk.call('tk_getOpenFile', '-foobarbaz')
-        except tk.TclError:
-            pass
-
-        window.tk.call('set', '::tk::dialog::file::showHiddenBtn', '1')
-        window.tk.call('set', '::tk::dialog::file::showHiddenVar', '0')
-    except:
-        pass
-
-    main_frame = tk.Frame(master=window)
-
-    raw_dir_lbl = tk.Label(master=main_frame, text="No directory selected", justify='left')
-    get_raw_dir_btn = tk.Button(master=main_frame, text="Select image directory",
-        command=partial(gui.get_image_dirname, raw_dir_lbl), width=20)
-
-    template_lbl = tk.Label(master=main_frame, text="Template file not selected", justify='left')
-    get_template_btn = tk.Button(master=main_frame, text="Select seed template", command=partial(gui.get_template_file, template_lbl), width=20)
-
-    out_dir_lbl = tk.Label(master=main_frame, text="Output directory: " + gui.state['paths']['out_dir'], justify='left')
-    get_out_dir_btn = tk.Button(master=main_frame, text="Select output directory",
-        command=partial(gui.get_out_dirname, out_dir_lbl), width=20)
-
-    save_btn = tk.Button(master=main_frame, text="Save settings", command=gui.save_state_dialog)
-    tweak_lbl = tk.Label(master=main_frame, text="Set recognition parameters: \n blur and color ranges", justify='left')
-    tweak_btn = tk.Button(master=main_frame, text="Recognition settings", command=partial(gui.tweak_image, window), width=20)
-
-    rotation_lbl = tk.Label(master=main_frame, text="Rotation angle: " + str(gui.state['rotation'].get()), justify='left')
-    rotation_btn = tk.Button(master=main_frame, text="Rotate image", command=partial(gui.rotation, window, rotation_lbl), width=20)
-
-    label_dict = {'input': raw_dir_lbl, 'template': template_lbl, 'outdir': out_dir_lbl, 'rotation': rotation_lbl}
-    load_btn = tk.Button(master=main_frame, text="Load settings", command=partial(gui.load_state_dialog, label_dict))
-
-
-    paper_size = tk.Entry(master=main_frame, width=20, textvariable=gui.state['paper_area'])
-    paper_size_lbl = tk.Label(master=main_frame, text="Paper size, mm^2", width=20)
-
-    germ_threshold = tk.Entry(master=main_frame, text="Germination threshold, mm", width=20, textvariable=gui.state['germ_thresh'])
-    germ_threshold_lbl = tk.Label(master=main_frame, text="Germination threshold, mm", width=28)
-    
-    seed_margin_width = tk.Entry(master=main_frame, text="Germination threshold, mm", width=20, textvariable=gui.state['seed_margin_width'])
-    seed_margin_width_lbl = tk.Label(master=main_frame, text="Seed margin width, %", width=28)
-
-    report_area = st.ScrolledText(main_frame, width=60, height=20, state=tk.DISABLED)
-    handler = gui.LoggingToGUI(report_area)
-    formatter = logging.Formatter('{levelname:>8}: {asctime} {message}',
-                datefmt='[%H:%M:%S]', style='{')
-    handler.setFormatter(formatter)
-    logger.addHandler(handler)
-    logger.setLevel(logging.DEBUG)
-    stream_handler = logging.StreamHandler()
-    stream_handler.setLevel(logging.DEBUG)
-    logger.addHandler(stream_handler)
-    stream_handler.setFormatter(formatter)
-    logging.getLogger('matplotlib').setLevel(logging.WARNING)
-
-    pb = ttk.Progressbar(main_frame, orient=tk.HORIZONTAL, mode='determinate', length=100, variable=gui.state['progress'])
-    pb_lbl = gui.FormatLabel(main_frame, textvariable=gui.state['progress'], format='{}%')
-
-    worker = threading.Thread(target=Morley.search, name='morley-worker')
-    run_btn = tk.Button(master=main_frame, text="RUN", command=worker.start, width=20)
-
-    gui.conditions.register({
-        'rotate': [rotation_btn],
-        'run': [run_btn],
-        'tweak': [tweak_btn]
-        })
-    for name in ['germ_thresh', 'paper_area']:
-        gui.state[name].trace('w', gui.trace_entry(name))
-        gui.state[name].set(gui.state[name].get())  # trigger trace functions
-
-    main_frame.grid(sticky=tk.N+tk.E+tk.S+tk.W)
-    get_raw_dir_btn.grid(column=0, row=1)
-    raw_dir_lbl.grid(column=1, row=1)
-
-    template_lbl.grid(row=2, column=1)
-    get_template_btn.grid(row=2, column=0)
-
-    get_out_dir_btn.grid(column=0, row=3)
-    out_dir_lbl.grid(column=1, row=3)
-
-    rotation_btn.grid(column=0, row=6)
-    rotation_lbl.grid(column=1, row=6)
-    load_btn.grid(column=0, row=0)
-
-    tweak_btn.grid(column=0, row=7)
-    tweak_lbl.grid(column=1, row=7)
-    save_btn.grid(column=1, row=0)
-
-    paper_size_lbl.grid(column=1, row=8)
-    paper_size.grid(column=0, row=8)
-
-    germ_threshold_lbl.grid(column=1, row=9)
-    germ_threshold.grid(column=0, row=9)
-    
-    seed_margin_width_lbl.grid(column=1, row=10)
-    seed_margin_width.grid(column=0, row=10)
-    
-    run_btn.grid(column=1, row=11)
-
-    report_area.grid(column=2, row=0, rowspan=11)
-    pb.grid(column=2, row=12)
-    pb_lbl.grid(column=2, row=13)
-
-    for col in range(3):
-        main_frame.columnconfigure(col, weight=1)
-
-    window.rowconfigure(0, weight=1)
-    window.columnconfigure(0, weight=1)
-    window.mainloop()
-    if worker.is_alive():
-        worker.join()
-    sys.exit()
-
-
-def main():
-    if len(sys.argv) == 1:
-        return start_gui()
-
-    formatter = logging.Formatter('{levelname:>8}: {asctime} {message}',
-                datefmt='[%H:%M:%S]', style='{')
-    stream_handler = logging.StreamHandler()
-    stream_handler.setLevel(logging.DEBUG)
-    logger.addHandler(stream_handler)
-    stream_handler.setFormatter(formatter)
-    logging.getLogger('matplotlib').setLevel(logging.WARNING)
-    logger.setLevel(logging.DEBUG)
-
-    parser = argparse.ArgumentParser(description="Morley CLI: run a Morley analysis in headless mode. ",
-        epilog="To use a GUI instead, run morley without any arguments.")
-    parser.add_argument('config', help="A JSON file with settings. You can obtain one by saving settings from GUI mode. "
-        "Other arguments override the values in config.")
-    parser.add_argument('-i', '--input', help="Input directory.")
-    parser.add_argument('-t', '--template', help="Template file.")
-    parser.add_argument('-o', '--output-dir', help="Output directory.")
-    parser.add_argument('-r', '--rotation', help='Input photo rotation.', type=int, choices=[0, 90, 180, 270])
-    parser.add_argument('-a', '--paper-area', help="Paper area, mm^2.", type=int)
-    parser.add_argument('-g', '--threshold', help="Germination threshold, mm.", type=int)
-    args = parser.parse_args()
-    gui.load_state_headless(args.config)
-    if args.input:
-        gui.state['paths']['input'] = args.input
-    if args.template:
-        gui.state['paths']['template_file'] = args.template
-    if args.output_dir:
-        gui.state['paths']['out_dir'] = args.output_dir
-    if args.rotation:
-        gui.state['rotation'].set(args.rotation)
-    if args.paper_area:
-        gui.state['paper_area'].set(args.paper_area)
-    if args.threshold:
-        gui.state['germ_thresh'].set(args.threshold)
-
-    gui.conditions.check_conditions()
-
-    missing = [c for c in gui.conditions.CONDITIONS['run'] if c not in gui.conditions.satisfied]
-    if missing:
-        logger.error("The following parameters are missing: %s", ', '.join(missing))
-        sys.exit(1)
-    Morley.search()
-
-
-if __name__ == '__main__':
-    main()
+import tkinter as tk
+from tkinter import ttk
+import tkinter.scrolledtext as st
+from idlelib.tooltip import Hovertip
+import logging
+from functools import partial
+import os
+import sys
+import threading
+import argparse
+import traceback
+from . import gui, Morley, version
+
+logger = logging.getLogger()
+
+
+def run_morley():
+    try:
+        Morley.search()
+    except Exception as e:
+        for line in traceback.format_exception(e):
+            logger.critical(line)
+        logger.critical('Fatal error occurred. Execution stopped.')
+
+
+def reset(button):
+    button['state'] = tk.NORMAL
+    button['text'] = 'RUN'
+    button['command'] = partial(start_morley, button)
+
+
+def stop_morley(button, worker):
+    gui.state['abort_flag'] = 1
+    button['state'] = tk.DISABLED
+
+
+def monitor(button, worker):
+    worker.join()
+    reset(button)
+
+
+def start_morley(button):
+    gui.state['abort_flag'] = 0
+    worker = threading.Thread(target=run_morley, name='morley-worker')
+    worker.start()
+    button['text'] = 'STOP'
+    button['command'] = partial(stop_morley, button, worker)
+    mon_t = threading.Thread(target=monitor, args=(button, worker), name='morley-monitor')
+    mon_t.start()
+
+
+def start_gui():
+    window = tk.Tk()
+    path_to_icon = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'logo.png')
+    window.tk.call('wm', 'iconphoto', window._w, tk.PhotoImage(file=path_to_icon))
+    # Add image file
+    background_image = tk.PhotoImage(path_to_icon)
+    background_label = tk.Label(window, image=background_image)
+    background_label.place(x=0, y=0, relwidth=1, relheight=1)
+    background_label.image = background_image
+
+    window.title(f'Morley GUI v{version.version}')
+    window.geometry('960x430')
+
+    gui.set_state_variables(gui.state)
+
+    # https://stackoverflow.com/a/54068050/1258041
+    try:
+        try:
+            window.tk.call('tk_getOpenFile', '-foobarbaz')
+        except tk.TclError:
+            pass
+
+        window.tk.call('set', '::tk::dialog::file::showHiddenBtn', '1')
+        window.tk.call('set', '::tk::dialog::file::showHiddenVar', '0')
+    except:
+        pass
+
+    main_frame = tk.Frame(master=window)
+
+    raw_dir_lbl = tk.Label(master=main_frame, text="No directory selected", justify='left')
+    get_raw_dir_btn = tk.Button(master=main_frame, text="Select image directory",
+        command=partial(gui.get_image_dirname, raw_dir_lbl), width=20)
+
+    template_lbl = tk.Label(master=main_frame, text="Template file not selected", justify='left')
+    get_template_btn = tk.Button(master=main_frame, text="Select seed template", command=partial(gui.get_template_file, template_lbl), width=20)
+
+    out_dir_lbl = tk.Label(master=main_frame, text="Output directory: " + gui.state['paths']['out_dir'], justify='left')
+    get_out_dir_btn = tk.Button(master=main_frame, text="Select output directory",
+        command=partial(gui.get_out_dirname, out_dir_lbl), width=20)
+
+    save_btn = tk.Button(master=main_frame, text="Save settings", command=gui.save_state_dialog)
+    tweak_lbl = tk.Label(master=main_frame, text="Set recognition parameters: \n blur and color ranges", justify='left')
+    tweak_btn = tk.Button(master=main_frame, text="Recognition settings", command=partial(gui.tweak_image, window), width=20)
+
+    rotation_lbl = tk.Label(master=main_frame, text="Rotation angle: " + str(gui.state['rotation'].get()), justify='left')
+    rotation_btn = tk.Button(master=main_frame, text="Rotate image", command=partial(gui.rotation, window, rotation_lbl), width=20)
+
+    label_dict = {'input': raw_dir_lbl, 'template': template_lbl, 'outdir': out_dir_lbl, 'rotation': rotation_lbl}
+    load_btn = tk.Button(master=main_frame, text="Load settings", command=partial(gui.load_state_dialog, label_dict))
+
+
+    paper_size = tk.Entry(master=main_frame, width=20, textvariable=gui.state['paper_area'])
+    paper_size_lbl = tk.Label(master=main_frame, text="Paper size, mm^2", width=20)
+
+    germ_threshold = tk.Entry(master=main_frame, text="Germination threshold, mm", width=20, textvariable=gui.state['germ_thresh'])
+    germ_threshold_lbl = tk.Label(master=main_frame, text="Germination threshold, mm", width=28)
+
+    seed_margin_width = tk.Checkbutton(master=main_frame, width=20, variable=gui.state['is_seed_big'])
+    seed_margin_width_lbl = tk.Label(master=main_frame, text="Shoot length is less or equal to the seeds max width", width=40)
+    
+    report_area = st.ScrolledText(main_frame, width=60, height=20, state=tk.DISABLED)
+    handler = gui.LoggingToGUI(report_area)
+    formatter = logging.Formatter('{levelname:>8}: {asctime} {message}',
+                datefmt='[%H:%M:%S]', style='{')
+    handler.setFormatter(formatter)
+    logger.addHandler(handler)
+    logger.setLevel(logging.DEBUG)
+    stream_handler = logging.StreamHandler()
+    stream_handler.setLevel(logging.DEBUG)
+    logger.addHandler(stream_handler)
+    stream_handler.setFormatter(formatter)
+    logging.getLogger('matplotlib').setLevel(logging.WARNING)
+
+    pb = ttk.Progressbar(main_frame, orient=tk.HORIZONTAL, mode='determinate', length=100, variable=gui.state['progress'])
+    pb_lbl = gui.FormatLabel(main_frame, textvariable=gui.state['progress'], format='{}%')
+
+    run_btn = tk.Button(master=main_frame, text="RUN", width=20)
+    run_btn['command'] = partial(start_morley, run_btn)
+
+    gui.conditions.register({
+        'rotate': [rotation_btn],
+        'run': [run_btn],
+        'tweak': [tweak_btn]
+        })
+    for name in ['germ_thresh', 'paper_area']:
+        gui.state[name].trace('w', gui.trace_entry(name))
+        gui.state[name].set(gui.state[name].get())  # trigger trace functions
+
+    for w in [paper_size, germ_threshold]:
+        Hovertip(w,'Enter an integer number.')
+
+    main_frame.grid(sticky=tk.N+tk.E+tk.S+tk.W)
+    get_raw_dir_btn.grid(column=0, row=1)
+    raw_dir_lbl.grid(column=1, row=1)
+
+    template_lbl.grid(row=2, column=1)
+    get_template_btn.grid(row=2, column=0)
+
+    get_out_dir_btn.grid(column=0, row=3)
+    out_dir_lbl.grid(column=1, row=3)
+
+    rotation_btn.grid(column=0, row=6)
+    rotation_lbl.grid(column=1, row=6)
+    load_btn.grid(column=0, row=0)
+
+    tweak_btn.grid(column=0, row=7)
+    tweak_lbl.grid(column=1, row=7)
+    save_btn.grid(column=1, row=0)
+
+    paper_size_lbl.grid(column=1, row=8)
+    paper_size.grid(column=0, row=8)
+
+    germ_threshold_lbl.grid(column=1, row=9)
+    germ_threshold.grid(column=0, row=9)
+
+    seed_margin_width_lbl.grid(column=1, row=10)
+    seed_margin_width.grid(column=0, row=10)
+
+    run_btn.grid(column=1, row=11)
+
+    report_area.grid(column=2, row=0, rowspan=11)
+    pb.grid(column=2, row=12)
+    pb_lbl.grid(column=2, row=13)
+
+    for col in range(3):
+        main_frame.columnconfigure(col, weight=1)
+
+    window.rowconfigure(0, weight=1)
+    window.columnconfigure(0, weight=1)
+    window.mainloop()
+    sys.exit()
+
+
+def main():
+    if len(sys.argv) == 1:
+        return start_gui()
+
+    formatter = logging.Formatter('{levelname:>8}: {asctime} {message}',
+                datefmt='[%H:%M:%S]', style='{')
+    stream_handler = logging.StreamHandler()
+    stream_handler.setLevel(logging.DEBUG)
+    logger.addHandler(stream_handler)
+    stream_handler.setFormatter(formatter)
+    logging.getLogger('matplotlib').setLevel(logging.WARNING)
+    logger.setLevel(logging.DEBUG)
+
+    parser = argparse.ArgumentParser(description="Morley CLI: run a Morley analysis in headless mode. ",
+        epilog="To use a GUI instead, run morley without any arguments.")
+    parser.add_argument('config', help="A JSON file with settings. You can obtain one by saving settings from GUI mode. "
+        "Other arguments override the values in config.")
+    parser.add_argument('-i', '--input', help="Input directory.")
+    parser.add_argument('-t', '--template', help="Template file.")
+    parser.add_argument('-o', '--output-dir', help="Output directory.")
+    parser.add_argument('-r', '--rotation', help='Input photo rotation.', type=int, choices=[0, 90, 180, 270])
+    parser.add_argument('-a', '--paper-area', help="Paper area, mm^2.", type=int)
+    parser.add_argument('-g', '--threshold', help="Germination threshold, mm.", type=int)
+    args = parser.parse_args()
+    gui.load_state_headless(args.config)
+    if args.input:
+        gui.state['paths']['input'] = args.input
+    if args.template:
+        gui.state['paths']['template_file'] = args.template
+    if args.output_dir:
+        gui.state['paths']['out_dir'] = args.output_dir
+    if args.rotation:
+        gui.state['rotation'].set(args.rotation)
+    if args.paper_area:
+        gui.state['paper_area'].set(args.paper_area)
+    if args.threshold:
+        gui.state['germ_thresh'].set(args.threshold)
+
+    gui.conditions.check_conditions()
+
+    missing = [c for c in gui.conditions.CONDITIONS['run'] if c not in gui.conditions.satisfied]
+    if missing:
+        logger.error("The following parameters are missing: %s", ', '.join(missing))
+        sys.exit(1)
+
+    gui.state['abort_flag'] = 0
+    Morley.search()
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `morley-0.0.4/morley.egg-info/PKG-INFO` & `morley-0.0.5/morley.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: morley
-Version: 0.0.4
+Version: 0.0.5
 Summary: GUI software for plant morphometry
 Home-page: UNKNOWN
 Author: Daria Emekeeva & Lev Levitsky
 Author-email: dashabezik65@gmail.com
 License: License :: OSI Approved :: Apache Software License
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Intended Audience :: End Users/Desktop
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # Morley
 
 Morley is open-sourse software for plants morphometry: measuring sprouts, roots length, plants area. Morley github repository is [here](https://github.com/dashabezik/Morley)
 
 # Overview
```

### Comparing `morley-0.0.4/setup.py` & `morley-0.0.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,20 +15,21 @@
             delim = '"' if '"' in line else "'"
             return line.split(delim)[1]
     else:
         raise RuntimeError("Unable to find version string.")
 
 setup(
     name                 = 'morley',
-    version              = get_version('morley/version.py'),
+    version              = '0.0.5',#get_version('morley/version.py'),
     description          = '''GUI software for plant morphometry''',
     long_description     = (''.join(open('pypi_md.md').readlines())),
     long_description_content_type="text/markdown",
     author               = 'Daria Emekeeva & Lev Levitsky',
     author_email         = 'dashabezik65@gmail.com',
+    python_requires      = '>=3.9',
     install_requires     = ['pyteomics', 'seaborn', 'scipy', 'scikit-learn', 'opencv-python', 'imutils'],
     classifiers          = ['Intended Audience :: Science/Research',
                             'Programming Language :: Python :: 3',
                             'Topic :: Scientific/Engineering :: Bio-Informatics',
                             'Intended Audience :: End Users/Desktop'],
     license              = 'License :: OSI Approved :: Apache Software License',
     packages             = find_packages(),
```

