# Comparing `tmp/pycol_complexity-0.0.5.tar.gz` & `tmp/pycol_complexity-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycol_complexity-0.0.5.tar", last modified: Sat Apr 20 09:55:29 2024, max compression
+gzip compressed data, was "pycol_complexity-0.0.6.tar", last modified: Wed May  1 10:43:30 2024, max compression
```

## Comparing `pycol_complexity-0.0.5.tar` & `pycol_complexity-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 09:55:29.858829 pycol_complexity-0.0.5/
--rw-rw-rw-   0        0        0     1103 2024-04-09 05:21:21.000000 pycol_complexity-0.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0     5569 2024-04-20 09:55:29.858829 pycol_complexity-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     5104 2024-03-21 06:37:06.000000 pycol_complexity-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-20 09:55:29.837396 pycol_complexity-0.0.5/pycol_complexity/
--rw-rw-rw-   0        0        0        0 2024-03-21 03:21:50.000000 pycol_complexity-0.0.5/pycol_complexity/__init__.py
--rw-rw-rw-   0        0        0    96143 2024-04-20 09:41:29.000000 pycol_complexity-0.0.5/pycol_complexity/complexity.py
-drwxrwxrwx   0        0        0        0 2024-04-20 09:55:29.857830 pycol_complexity-0.0.5/pycol_complexity.egg-info/
--rw-rw-rw-   0        0        0     5569 2024-04-20 09:55:29.000000 pycol_complexity-0.0.5/pycol_complexity.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2024-04-20 09:55:29.000000 pycol_complexity-0.0.5/pycol_complexity.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 09:55:29.000000 pycol_complexity-0.0.5/pycol_complexity.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-20 09:55:29.000000 pycol_complexity-0.0.5/pycol_complexity.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      215 2024-03-21 04:48:10.000000 pycol_complexity-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0      559 2024-04-20 09:55:29.860826 pycol_complexity-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-01 10:43:30.606247 pycol_complexity-0.0.6/
+-rw-rw-rw-   0        0        0     1103 2024-04-09 05:21:21.000000 pycol_complexity-0.0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0     5569 2024-05-01 10:43:30.606247 pycol_complexity-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     5104 2024-03-21 06:37:06.000000 pycol_complexity-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 10:43:30.577002 pycol_complexity-0.0.6/pycol_complexity/
+-rw-rw-rw-   0        0        0        0 2024-03-21 03:21:50.000000 pycol_complexity-0.0.6/pycol_complexity/__init__.py
+-rw-rw-rw-   0        0        0   105323 2024-05-01 10:41:10.000000 pycol_complexity-0.0.6/pycol_complexity/complexity.py
+drwxrwxrwx   0        0        0        0 2024-05-01 10:43:30.605235 pycol_complexity-0.0.6/pycol_complexity.egg-info/
+-rw-rw-rw-   0        0        0     5569 2024-05-01 10:43:30.000000 pycol_complexity-0.0.6/pycol_complexity.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2024-05-01 10:43:30.000000 pycol_complexity-0.0.6/pycol_complexity.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 10:43:30.000000 pycol_complexity-0.0.6/pycol_complexity.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-01 10:43:30.000000 pycol_complexity-0.0.6/pycol_complexity.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      215 2024-03-21 04:48:10.000000 pycol_complexity-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0      559 2024-05-01 10:43:30.608967 pycol_complexity-0.0.6/setup.cfg
```

### Comparing `pycol_complexity-0.0.5/LICENSE.txt` & `pycol_complexity-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pycol_complexity-0.0.5/PKG-INFO` & `pycol_complexity-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycol_complexity
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python Package for complexity measures
 Home-page: https://github.com/DiogoApostolo/pycol
 Author: Diogo Apostolo
 Author-email: ogoid.478@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pycol_complexity-0.0.5/README.md` & `pycol_complexity-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pycol_complexity-0.0.5/pycol_complexity/complexity.py` & `pycol_complexity-0.0.6/pycol_complexity/complexity.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import sklearn
 from sklearn.metrics import DistanceMetric
 import sklearn.pipeline
 import scipy.spatial
 import pandas as pd
 
 
-from catboost.datasets import epsilon,higgs,adult
+
 
 import pickle
 
 
 
 
 
@@ -46,16 +46,18 @@
         file_type (string): The type of file where the dataset is stored. Only available option right now is "arff" and "pickle".
         
         '''
         if(file_type=="arff"):
             [X,y,meta]=self.__read_file(file_name)
         elif(file_type=="pickle"):
             [X,y,meta]=self.__prepare_array(file_name)
+        elif(file_type=="csv"):
+            [X,y,meta]=self.__read_csv(file_name)
         else:
-            print("Only arff files are available for now")
+            print("Only arff and pickle files are available for now")
             return
 
         self.X=np.array(X)
       
         self.y=np.array(y)
         classes=np.unique(self.y)
 
@@ -99,15 +101,15 @@
             if meta[i]==1:
                 label_encoder = LabelEncoder()
                 # Fit the LabelEncoder to your categorical values and transform them to numerical values
                 numerical_values = label_encoder.fit_transform(X[:,i])
                 X[:,i] = numerical_values
 
         if 1 in meta:
-            X = X.astype(np.float64)
+            X = X.astype(float)
 
         return X
 
     def is_categorical(self,X):
         meta = []
         # Iterate through each column in the array
         for i in range(X.shape[1]):
@@ -128,15 +130,15 @@
         
 
 
         #change this
         with open(dataset_name, 'rb') as f:
             epsilon_train = pickle.load(f)
 
-        print(epsilon_train)
+        
         X = epsilon_train[:,0:len(epsilon_train[0])-1]
         y = epsilon_train[:,-1]
 
         meta = self.is_categorical(X)
 
         X = self.encode(X,meta)
 
@@ -147,14 +149,49 @@
         y = [np.where(classes == i)[0][0] for i in y]
         
 
              
 
         return [X,y,meta]
     
+    def __convert_columns_to_float(self,arr):
+        num_cols = arr.shape[1]
+        converted_arr = np.empty_like(arr, dtype=float)
+        
+        for i in range(num_cols):
+            try:
+                converted_arr[:, i] = arr[:, i].astype(float)
+            except ValueError:
+                converted_arr[:, i] = arr[:, i]
+        
+        return converted_arr
+
+
+    def __read_csv(self,dataset_name):
+        data = np.genfromtxt(dataset_name, delimiter=',', dtype=None, encoding=None)
+        
+        #skip header start at 1
+        X = data[1:,0:len(data[0])-1]
+        y = data[1:,-1]
+        meta = self.is_categorical(X)
+
+        
+
+        X = self.encode(X,meta)
+
+        X = self.__convert_columns_to_float(X)
+
+        
+        #indentify the existing classes
+        classes = np.unique(y)
+
+        #create new class labels from 0 to n, where n is the number of classes
+        y = [np.where(classes == i)[0][0] for i in y]
+        return [np.array(X),np.array(y),meta]
+
     
     def __read_file(self,file_name):
         '''
         Is called by the __init__ method.
         Read an arff file containing the dataset.
         --------
         Parameters:
@@ -371,15 +408,15 @@
         class_inds = []
         for cls in self.classes:
             cls_ind=np.where(self.y==cls)[0]
             class_inds.append(cls_ind)
         return class_inds
 
 
-    def __knn(self,inx,line,k,clear_diag=True):
+    def __knn(self,inx,line,k,y=[],clear_diag=True):
         '''
         Called by all the complexity metrics that need to calculate the nearest neighbours of a sample.
         Calculates the class labels of the k nearest neighbours of a sample x. If clear_diag is True, it is assumed that point in
         position "inx" is the sample x, which will have distance 0 to itself and so the distance is changed to infinite to avoid
         one of the nearest neighbours being the point itself.
         --------
         Parameters:
@@ -389,22 +426,26 @@
         clear_diag (bool): True if the distance in position "inx" of "line" is the point itself.
         --------
         Returns:
         count: An (n*1) array, where n is the number of unique class labels, where in each position is the value of how many of the k
         nearest neighbours belong to that class. For example if k=5 and there are 3 classes a possible configuration could be [2,3,0] meaning that 2
         of the neighbours are from the 1st class, 3 are from the second class, and there are none from the 3rd class.
         '''
+        
+        if(len(y)==0):
+            y = self.y
+        
         count = np.zeros(len(self.classes))
         if(clear_diag):
             line[inx]=math.inf
         for i in range(k):
             index=np.where(line == min(line))[0][0]
             line[index]=math.inf
             #if(self.y[index]!=self.y[inx]):
-            cls_inx = np.where( self.classes == self.y[index])[0][0]  
+            cls_inx = np.where( self.classes == y[index])[0][0]  
             count[cls_inx]+=1
 
         return count
     
 
     def __knn_dists(self,inx,line,k,clear_diag=True):
         dists = []
@@ -682,35 +723,55 @@
         
         '''
         sum_val = 0
         m = len(profile)
         for j in range(m):
             w = (1-(j/m))
             sum_val += w * (1-profile[j])
-        mri_val = sum_val*(1/(2*m))
+        mri_val = sum_val/(2*m)
     
         return mri_val
 
+    
+    def count_occurences(self,labels):
+        occurrences = {}
+        for label in labels:
+            if label in occurrences:
+                occurrences[label] += 1
+            else:
+                occurrences[label] = 1
+        return occurrences
+    
+    
     def __MRI_k(self,cluster):
         '''
         Called by the MRCA function. Calculates the Multiresolution Index (MRI) for a cluster by
         averaging the MRI value of each pattern in the cluster.
         --------
         Parameters:
         cluster (array): An array of arrays (N*M) containg all the points in a cluster, where N is the number of points and M is the 
         dimesion of each point.
         ---------
         Returns:
         mri_val (float): The multiresolution index of the cluster
         ---------
         '''
+
+        
+
+
         sum_val = 0
-        for profile in cluster:
+        for i in range(len(cluster)):
+            profile = cluster[i]
             sum_val+= self.__MRI_p(profile)
+        
+        
+        
         mri_val=sum_val/len(cluster)
+
         return mri_val
 
     def MRCA(self,sigmas=[0.25,0.5,0.75],n_clusters=3,distance_func="default"):
         '''
         Calculates the MRCA value complexity measure defined in [1].
 
         -------
@@ -764,26 +825,27 @@
                         #calculate the psi values for each profile in accordance to [1]
                         if(new_y[i]==c1):
                             alt_y = 1
                             psi = alt_y * ((n[1]-n[0])/(n[1]+n[0]))      
                         else:
                             alt_y = -1
                             psi = alt_y * ((n[0]-n[1])/(n[0]+n[1]))      
+
                         profiles[i,j]=psi
 
                 #cluster the the profiles
                 
                 kmeans = KMeans(n_clusters=n_clusters).fit(profiles)
                 
 
                 #for each cluster calculate the MRI value
                 for i in range(n_clusters):
                     inx = np.where( kmeans.labels_ == i)[0]
                     cluster = profiles[inx]
-                    
+                    labels = new_y[inx]
                     mrca[i]=self.__MRI_k(cluster)
 
                 return mrca
                 
     
 
     def C1(self,max_k=5,imb=False):
@@ -862,15 +924,18 @@
                 #which are not.
                 #n = self.__hypersphere(i,sigma)
                 
                 dists=self.__knn_dists(i,copy.copy(self.dist_matrix[i]),k)
             
                 pkj = 0
                 for d in dists:
-                    pkj+=1-d
+                    if(d > 1):
+                        d = 1
+
+                    pkj+= 1-d
                 pkj/= k
 
                 #cls_inx = np.where( self.classes == self.y[i])[0][0]
                 #pkj=count[cls_inx]/k
                 c2_instance_sum += pkj
 
             c2_instance_val = 1-(c2_instance_sum/max_k)
@@ -1331,15 +1396,15 @@
         var (bool): True if hypersphere a is inside hypersphere b, false if not.
         '''
         var = False
         
        
 
        
-        if(abs(np.sqrt(sum(np.square(center_a-center_b))) - (radius_b-radius_a))<0.01):
+        if(abs(np.sqrt(sum(np.square(center_a-center_b))) - (radius_b-radius_a))<0.001):
             
             var=True
         return var
 
     def _scale_N(self,N: np.ndarray) -> np.ndarray:
         """Scale all features of N to [0, 1] range."""
         N_scaled = N
@@ -1374,15 +1439,15 @@
             
            
             for inx2_sphere in inx_sorted[:inx1:-1]:
                 
                 if (self.__is_inside(X[inx1_sphere],X[inx2_sphere],radius[inx1_sphere],radius[inx2_sphere])):
                     
                     inst_per_sphere[inx2_sphere] += inst_per_sphere[inx1_sphere]
-                    inst_per_sphere[inx2_sphere] = 0
+                    inst_per_sphere[inx1_sphere] = 0
                     break
 
         return inst_per_sphere    
 
     
 
 
@@ -1425,81 +1490,114 @@
             ordered_radius = np.concatenate((ordered_radius,radius[self.class_inxs[i]]))
         '''
         
         return sphere_inst_count,radius
     
 
     #only for datasets with no categorical features
-    def T1(self):
+    def T1(self,imb=False):
         '''
         Calculate the T1 value complexity measure defined in [1].
-
+        -------
+        Parameters:
+        imb (bool): If True the the values for minority and majority will both be returned individually, if False a single value for the whole dataset is returned
         -------
         Returns: 
         t1 (float): The t1 complexity measure
         -------
         References:
 
         [1] Lorena AC, Garcia LP, Lehmann J, Souto MC, Ho TK (2019) How complex
         is your classification problem? a survey on measuring classification
         complexity. ACM Computing Surveys (CSUR) 52(5):1-34
         '''
         sphere_inst_count,radius=self.__get_sphere_count()
+
         
-        t1 = len(sphere_inst_count[sphere_inst_count > 0])/ len(self.y)
+
+        if(imb):
+            inx=np.where(sphere_inst_count!=0)[0]
+            num_inx_per_class = np.zeros(len(self.classes))
+            #count the number of hyperspheres of each class
+            for i in inx:
+                cls_inx = np.where( self.classes == self.y[i])[0][0]
+                num_inx_per_class[cls_inx]+=1
+
+            t1 = np.divide(num_inx_per_class, self.class_count)
+        
+        else:
+            t1 = len(sphere_inst_count[sphere_inst_count > 0])/ len(self.y)
         
         #t1 = sum(sphere_inst_count[sphere_inst_count > 0]) / len(self.y)))/len(sphere_inst_count[sphere_inst_count > 0])
         return t1
 
 
     #only for datasets with no categorical features
-    def DBC(self,distance_func="default"):
+    def DBC(self,distance_func="default",imb=False):
         '''
         Calculate the DBC complexity measure defined in [1].
 
         -------
         Parameters:
         distance_func (string): The distance metric to calculate the distance between all hypersphere centers. 
         For now this value can only be "HEOM", since this is the only distance metric implemented.
+        imb (bool): If True the the values for minority and majority will both be returned individually, if False a single value for the whole dataset is returned
         -------
         Returns:
         dbc_measure (float): the DBC complexity measure
         -------
         References:
 
         [1] Van der Walt CM, et al. (2008) Data measures that characterise
         classification problems. PhD thesis, University of Pretoria
 
         '''
 
         #find the hypersphere centers
         sphere_inst_count,radius=self.__get_sphere_count()
-        inx=np.where(sphere_inst_count!=0)
+        inx=np.where(sphere_inst_count!=0)[0]
+
+
+        num_inx_per_class = np.zeros(len(self.classes))
+
+        
+        if(imb):
+            #count the number of hyperspheres of each class
+            for i in inx:
+                cls_inx = np.where( self.classes == self.y[i])[0][0]
+                num_inx_per_class[cls_inx]+=1
+
         new_X = self.X[inx]
         new_y = self.y[inx]
 
         #calculate the distance between the hypersphere centers.
         new_dist_matrix,_ =self.__calculate_distance_matrix(new_X,distance_func=distance_func)
 
         #calculate the MST of using the hypersphere centers and find the number of vertixes linked by an edge in the MST that have a different class label
-        n_inter = self.__calculate_n_inter(dist_matrix=new_dist_matrix,y=new_y)
-      
-        dbc_measure = n_inter/len(sphere_inst_count[sphere_inst_count > 0])
+        n_inter = self.__calculate_n_inter(dist_matrix=new_dist_matrix,y=new_y,imb=imb)
+
 
+        if(imb):
+            dbc_measure = np.divide(n_inter,num_inx_per_class)
+        else:
+            dbc_measure = n_inter/len(sphere_inst_count[sphere_inst_count > 0])
+        
         
         return dbc_measure
 
     
     
     
     
-    def LSC(self):
+    def LSC(self,imb=False):
         '''
         Calculate the LSC measure defined in [1].
-
+        ------
+        Parameters:
+        imb (bool): If True the the values for minority and majority will both be returned individually, if False a single value for the whole dataset is returned
         ------
         Returns:
         lsc_measure (float): The value of the lsc complexity measure
         ------
         References:
 
         [1] Leyva E, González A, Perez R (2014) A set of complexity measures
@@ -1507,30 +1605,48 @@
         on Knowledge and Data Engineering 27(2):354-367
         '''
 
 
         #find the nearest neightbour of the oposite class for every sample
         nearest_enemy_inx,nearest_enemy_dist = self.__find_nearest_oposite_class_all()
         
-        ls_count = []
+        if(imb):
+            ls_count = []
+            for i in range(len(self.classes)):
+                ls_count.append([])
+        else:
+            ls_count = []
         
         #for each sample count the amount of samples inside the hypersphere centered at the sample with radius equal
         #to the distance to the nearest sample of the oposite class.
         for i in range(len(self.dist_matrix)):
             count = 0
             for j in range(len(self.dist_matrix[i])):
                 if(self.y[i]==self.y[j] and self.dist_matrix[i][j]<nearest_enemy_dist[i]):
                     count += 1
-            ls_count.append(count)
+            
+            if(imb):
+                cls_inx = np.where( self.classes == self.y[i])[0][0]
+                ls_count[cls_inx].append(count)
+            else:
+                ls_count.append(count)
+
 
-        lsc_measure = 1-sum(ls_count)/(len(self.X)**2)
+        if(imb):
+            ls_sum = []
+            for i in range(len(self.classes)):
+                ls_sum.append(sum(ls_count[i]))
+
+            lsc_measure = 1-(np.divide(ls_sum,self.class_count**2))
+        else:
+            lsc_measure = 1-(sum(ls_count)/(len(self.X)**2))
         return lsc_measure
 
 
-    def Clust(self):
+    def Clust(self,imb=False):
         '''
         Calculate the Clust complexity measure defined in [1].
 
         ------
         Returns:
         clust_measure (float): the value of the Clust complexity measure
 
@@ -1558,15 +1674,15 @@
                     inxs.append(j)
             cls_inx = np.where( self.classes == self.y[i])[0][0]
             
             ls_count[cls_inx].append((count,i,inxs))
         
      
         
-        core_count=0
+        core_count=np.zeros(len(self.classes))
         for i in range(len(ls_count)):
             clusters = []
             #sort all the classes LS
             ls_count[i].sort(key=itemgetter(0), reverse=True)
 
             
             for i2 in range(len(ls_count[i])):
@@ -1582,46 +1698,67 @@
                     clusterCoreInx = ls_count[i].index(ls_count[i][i2])
                     clusterCore = ls_count[i][i2]
                     clusterMembers = [clusterCore]
                     
                     cluster = [clusterCoreInx,clusterCore,clusterMembers]
                     clusters.append(cluster)
             #sum the number of cores
-            core_count+=len(clusters)    
+            core_count[i]=len(clusters)    
             
 
         
        
-
-        clust_measure = core_count/len(self.X)
+        if(imb):
+            clust_measure = np.divide(core_count,self.class_count)
+        else:
+            clust_measure = sum(core_count)/len(self.X)
         return clust_measure
 
     #only for datasets with no categorical features
-    def NSG(self):
+    def NSG(self,imb=False):
         '''
         Calculate the NSG complexity measure defined in [1].
-
+        -------
+        Parameters:
+        imb (bool): If True the the values for minority and majority will both be returned individually, if False a single value for the whole dataset is returned
         -------
         Returns: 
         nsg_measure (float): The value of the NSG complexity measure
         -------
         References:
 
         [1] Van der Walt CM, Barnard E (2007) Measures for the characterisation
         of pattern-recognition data sets. 18th Annual Symposium of the Pattern
         Recognition Association of South Africa
         '''
         sphere_inst_count,radius=self.__get_sphere_count()
+        
+
+        
+
+        if(imb):
+        #count the number of hyperspheres of each class
+            inx=np.where(sphere_inst_count!=0)[0]
+
 
+            num_inx_per_class = np.zeros(len(self.classes))
+            num_instances_per_ball_per_class = np.zeros(len(self.classes))
+            for i in inx:
 
-        nsg_measure = sum(sphere_inst_count)/len(sphere_inst_count[sphere_inst_count > 0])
+                cls_inx = np.where( self.classes == self.y[i])[0][0]
+                num_inx_per_class[cls_inx]+=1
+               
+
+            nsg_measure = np.divide(num_instances_per_ball_per_class,num_inx_per_class)
+        else:
+            nsg_measure = sum(sphere_inst_count)/len(sphere_inst_count[sphere_inst_count > 0])
         return nsg_measure
     
     #only for datasets with no categorical features
-    def ICSV(self):
+    def ICSV(self,normalize=True,imb=False):
         
         '''
         Calculate the ICSV complexity measure defined in [1].
 
         -------
         Returns: 
         icsv_measure (float): The value of the ICSV complexity measure
@@ -1633,40 +1770,53 @@
         Recognition Association of South Africa
         
         '''
         
         #find the hyperspheres and their radius
         sphere_inst_count,radius=self.__get_sphere_count()
         
+        inx=np.where(sphere_inst_count!=0)[0]
         
+        #keep only the hyperspheres with samples in them
+        sphere_inst_count_non_zero = sphere_inst_count[inx] 
+        radius_non_zero = radius[inx]
+
+        if(normalize):
+            radius_non_zero = radius_non_zero/np.max(radius_non_zero)
 
         #calculate the density of each hypersphere
-        n = len(self.class_inxs)
+        n = len(self.X[0])
         density = []
-        for i in range(len(radius)):
-            #volume = 4/3 * math.pi* radius[i] **3
-            volume = (math.pi**(n/2)/math.gamma(n/2 + 1)) * radius[i]**n
-            density.append(sphere_inst_count[i]/volume)
-            
+        volumes = []
+        for i in range(len(sphere_inst_count_non_zero)):
+            volumes.append((math.pi**(n/2)/math.gamma(n/2 + 1)) * radius_non_zero[i]**n)
+    
         
-        icsv_measure = 0
-
+        
+        for i in range(len(sphere_inst_count_non_zero)):
 
-        mean = sum(density)/len(sphere_inst_count[sphere_inst_count > 0])
-       
+            density.append(sphere_inst_count_non_zero[i]/volumes[i])
+            
         
-        #calculate the icsv measure using the mean and densities of the spheres
-        for i in range(len(radius)):
-           if(density[i]!=0):
-                icsv_measure+=(density[i]-mean)**2
         
-
-
-        icsv_measure = icsv_measure/len(sphere_inst_count[sphere_inst_count > 0])
-        icsv_measure = math.sqrt(icsv_measure)
+        if(imb):
+            density_per_class = []
+            for i in range(len(self.classes)):
+                density_per_class.append([])
+            j = 0
+            for i in range(len(sphere_inst_count)):
+                if(sphere_inst_count[i]!=0):
+                    cls_inx = np.where( self.classes == self.y[i])[0][0]
+                    density_per_class[cls_inx].append(density[j])
+                    j+=1
+            icsv_measure = []
+            for i in range(len(self.classes)):
+                icsv_measure.append(np.std(density_per_class[i]))
+        else:
+            icsv_measure = np.std(density)
 
         return icsv_measure
 
     def __calculate_cells(self,resolution,transpose_X,get_labels=0):
         '''
         Called py the purity and neighbourhood_separability functions.
         Creates a dictionary that maps each of the cells to the samples inside it. or if get_lables=1 it
@@ -1692,28 +1842,37 @@
           
             
            
 
               
             step = (max_feature-min_feature)/(resolution+1)
             steps.append(step)
+
+
             #calculate the hypercube bounds for each dimension
+            if(step==0):
+                feature_bounds.append([min_feature,max_feature])
+            else:
+                feature_bounds.append(np.linspace(min_feature,max_feature,num=2+resolution))
+            
             
-            feature_bounds.append(np.arange(min_feature,max_feature,step))
-        
-
         
        
         sample_dic = {}
-        #map each cell to the cell it belongs to (sample->cell)
+        #map each cell to the cell it belongs to (sample->cell). In the case of 2 features if sample is mapped to 0-0 it means it's in the first interval for both features
+        #if the sample is mapped to 1-0, then it means it's in the second iterval for the first feature and in the first interval of the second feature
+        
+        #for each sample
         for s in range(len(self.X)):
             sample = self.X[s]
+            #for each feature value of the sample
             for j in range(len(self.X[0])):
+                #determine in which interval the value bellongs to for this feature
                 for k in range(len(feature_bounds[j])):
-                
+                    #if the sample is inside this cell
                     if(sample[j]>=feature_bounds[j][k] and sample[j]<=feature_bounds[j][k]+steps[j]):
                         if(str(s) not in sample_dic):
                             sample_dic[str(s)]=""+str(k)
                         else:
                             sample_dic[str(s)]+="-"+str(k)
                         break
         
@@ -1728,26 +1887,28 @@
 
         
         for inx in self.class_inxs:
             plt.plot(self.X[inx,0],self.X[inx,1],"o",markersize=4)
         plt.show()
         '''
 
-        #reverse the mapping (cell->sample)
+        #reverse the mapping (cell->sample) if get_labels == 1 then instead of the mapping the cells to the samples it maps cells to class labels as well
         reverse_dic = {}
+        reverse_dic_labels = {}
         for k,v in sample_dic.items():
             reverse_dic[v]= reverse_dic.get(v,[])
+            reverse_dic_labels[v]= reverse_dic_labels.get(v,[])
             #values are the class lables 
             if(get_labels==1):
-                reverse_dic[v].append(self.y[int(k)]) 
-            else:
-                reverse_dic[v].append(int(k)) 
+                reverse_dic_labels[v].append(self.y[int(k)]) 
+            
+            reverse_dic[v].append(int(k)) 
 
         
-        return reverse_dic
+        return reverse_dic_labels,reverse_dic
 
 
     #only for datasets with no categorical features
     def purity(self,max_resolution=32):
         '''
         Calculates the purity complexity measure defined in [1].
 
@@ -1756,23 +1917,23 @@
         max_resolution (int): the maximum resolution to consider to divide the feature space. The function will iterate from 0 (no partitioning) to max_resolution.
         -----
         Returns: 
         auc (float): Corresponds to the value of the purity complexity measure.
         -----
         References:
 
-        [1] Singh S (2003) Prism{a novel framework for pattern recognition. Pattern
+        [1] Singh S (2003) Prism: a novel framework for pattern recognition. Pattern
         Analysis & Applications 6(2):134-149
 
         '''
         transpose_X = np.transpose(self.X)
         purities = [] 
         #multiple resolutions
         for i in range(max_resolution):
-            reverse_dic=self.__calculate_cells(i,transpose_X,get_labels=1)
+            reverse_dic,__=self.__calculate_cells(i,transpose_X,get_labels=1)
             purity = 0
             #calculate purity
             for cell in reverse_dic:
                 
                 classes = self.classes
                 class_counts = [0]*len(classes)
                 num_classes = len(classes)
@@ -1795,15 +1956,15 @@
             purities.append(purity)
         
         w_purities = []
         for i in range(len(purities)):
             new_p = purities[i]*(1/2**(i))
             w_purities.append(new_p)
         
-        norm_resolutions = [x/max_resolution for x in list(range(max_resolution))]
+        norm_resolutions = [x/(max_resolution-1) for x in list(range(max_resolution))]
         norm_purities = [(x-min(w_purities))/(max(w_purities)-min(w_purities)) for x in w_purities]
         
         auc=sklearn.metrics.auc(norm_resolutions,norm_purities)
         return auc/0.702
     
 
     #only for datasets with no categorical features
@@ -1816,66 +1977,73 @@
         max_resolution (int): the maximum resolution to consider to divide the feature space. The function will iterate from 0 (no partitioning) to max_resolution.
         -----
         Returns: 
         final_auc (float): Corresponds to the value of the neighbourhood_separability complexity measure.
         -----
         References:
         
-        [1] Singh S (2003) Prism{a novel framework for pattern recognition. Pattern
+        [1] Singh S (2003) Prism: a novel framework for pattern recognition. Pattern
         Analysis & Applications 6(2):134-149
 
         '''
         transpose_X = np.transpose(self.X)
         neigh_sep = []
         #multiple resolutions
         for i in range(max_resolution):
             
-            reverse_dic=self.__calculate_cells(i,transpose_X)
-            reverse_dic_labels=self.__calculate_cells(i,transpose_X,get_labels=1)
+            
+            reverse_dic_labels,reverse_dic=self.__calculate_cells(i,transpose_X,get_labels=1)
             average_ns=0
             for cell in reverse_dic:
                 
                 average_auc=0
                 for sample in reverse_dic[cell]:
                     props = []
-                    same_class_num = len(np.where(reverse_dic_labels[cell] == self.y[sample])[0])
+
+                    #number of samples in this cell of the same class as this sample (minus itself)
+                    same_class_num = len(np.where(reverse_dic_labels[cell] == self.y[sample])[0])-1
                     
                     #according to the original paper limiting the max num to 11 is good practice since for large datasets the process
                     #becomes too costly
                     if(same_class_num>11):
                         same_class_num=11
 
-                    #does it still count itself?
+
                     for k in range(same_class_num):
                         #checks all neighbours and not just the ones the cell
-                        count=self.__knn(sample,copy.copy(self.dist_matrix[sample]),k+1)
+                        count=self.__knn(reverse_dic[cell].index(sample),copy.copy(self.dist_matrix[sample,reverse_dic[cell]]),k+1)
                         cls_inx = np.where( self.classes == self.y[sample])[0][0]
                         class_count=count[cls_inx]
                         
                         prop = class_count/sum(count)
                         props.append(prop)
                     
 
-                    #if the sample is the only one of its class in the cell
-                    if(len(props)<2):
-                        
+                    #if the sample is the only one of its class in the cell and there are samples of other classes in the cell
+                    if(len(props)==0 and len(reverse_dic[cell])>1):
                         auc=0
+                    #if the sample is the only one of its class in the cell and the only sample in the cell
+                    elif(len(props)==0 and len(reverse_dic[cell])==1):
+                        auc=1
+                    #if there is only one other sample if the same class
+                    elif(len(props)==1):
+                        auc = props[0]
                     else:
                         norm_k = [x/same_class_num for x in list(range(same_class_num))]
                         auc = sklearn.metrics.auc(norm_k, props)
                        
                     average_auc+=auc
                 average_auc/=len(reverse_dic[cell])
                 average_ns+=average_auc*(len(reverse_dic[cell])/len(self.X))
             neigh_sep.append(average_ns)
         w_neigh_sep = []
         for i in range(len(neigh_sep)):
             w_neigh_sep.append(neigh_sep[i]*(1/2**i))
         
-        norm_resolutions = [x/max_resolution for x in list(range(max_resolution))]
+        norm_resolutions = [x/(max_resolution-1) for x in list(range(max_resolution))]
         final_auc=sklearn.metrics.auc(norm_resolutions,w_neigh_sep)
         return final_auc
 
 
     #only for datasets with no categorical features
     def F1(self):
         '''
@@ -2338,14 +2506,60 @@
                 total_count=0
                 total_count+=self.__class_overlap(sample_c1,sample_c2)
                 total_count+=self.__class_overlap(sample_c2,sample_c1)
 
                 ins.append(total_count/(len(X)*len(X[0])))
         return ins
 
+    def input_noise_imb(self,imb=False):
+        '''
+        Calculate the input noise metric defined in [1].
+        Uses one vs one method if the dataset contains more than 2 classes.
+        -----
+        Returns:
+        ins (array): the input noise value for each each one vs one combination of classes.
+        -----
+        References:
+
+        [1] Van der Walt CM, Barnard E (2007) Measures for the characterisation
+        of pattern-recognition data sets. 18th Annual Symposium of the Pattern
+        Recognition Association of South Africa
+        '''
+        ins = []
+        for i in range(len(self.class_inxs)):
+            for j in range(i+1,len(self.class_inxs)):
+                X = self.X
+                valid_inxs_c1 = self.class_inxs[i]
+                valid_inxs_c2 = self.class_inxs[j]
+                sample_c1 = X[valid_inxs_c1]
+                sample_c2 = X[valid_inxs_c2]
+                
+
+
+                if(len(sample_c1)>len(sample_c2)):
+                    total_count_maj= self.__class_overlap(sample_c1,sample_c2)
+                    total_count_min= self.__class_overlap(sample_c2,sample_c1)
+                    sample_maj = sample_c1
+                    sample_min = sample_c2
+                else:
+                    total_count_min= self.__class_overlap(sample_c1,sample_c2)
+                    total_count_maj= self.__class_overlap(sample_c2,sample_c1)
+                    sample_min = sample_c1
+                    sample_maj = sample_c2
+
+                if(imb):
+                    ins.append([
+                                total_count_maj/(len(sample_maj)*len(X[0])), 
+                                total_count_min/(len(sample_min)*len(X[0]))
+                            ])
+                else:
+                    total_count = total_count_maj + total_count_min
+                    ins.append(total_count/(len(X)*len(X[0])))
+        return ins
+
     
 
     
     def borderline(self,k=5,imb=False):
         '''
         Calculates the borderline examples metric defined in [1].
 
@@ -2365,15 +2579,15 @@
         
         '''
         borderline_count = np.zeros(len(self.classes))
         for i in range(len(self.X)):
             count=self.__knn(i,copy.copy(self.dist_matrix[i]),k)
             cls_inx = np.where( self.classes == self.y[i])[0][0]
             #check this
-            if((sum(count)-count[cls_inx])>=2):
+            if( (sum(count)-count[cls_inx])>=2 ):
                 borderline_count[cls_inx]+=1
         
         if(imb):
             borderline = np.divide(borderline_count,self.class_count)
         else:
             borderline = sum(borderline_count)/len(self.X)
         
@@ -2414,33 +2628,37 @@
 
   
 
     # -*- coding: utf-8 -*-
 
 
 
-    def ONB_avg(self):
+    def ONB_avg(self,imb=False):
 
         """
 
         ONB complexity metric differentiating (averaged) by class
-
-
+        ------
+        Parameters:
+        imb (bool): If True the the values for minority and majority will both be returned individually, if False a single value for the whole dataset is returned
+        ------
+        Returns:
+        avg (float): The ratios between the number of balls necessary to cover the points of a class and the number of points of that class
         """
         featu = pd.DataFrame(self.X) #feature part of the dataframe
         
         clas = pd.DataFrame(self.y) #class part of the dataframe
         
         clas.rename(columns = {0 : 'class'}, inplace = True)
         
         dataset = featu.join(clas)
 
-        clas_dif = np.unique(clas) #array of the different clases in the dataset   
+        clas_dif = self.classes
 
-        
+        instance_per_ball = []
 
         dtf_dist =  pd.DataFrame(self.dist_matrix) #distance matrix as a dataframe    
 
         lista_el_cla = [] #empty list for the elements of each class
 
         el_cla = [] #empty list for the number of elements in each class
 
@@ -2448,16 +2666,20 @@
 
             lista_el_cla = lista_el_cla + [list(dataset.loc[dataset["class"]==cla].index.values)] #add the elements of each class
 
             el_cla = el_cla + [len(list(dataset.loc[dataset["class"]==cla].index.values))] #add the number of elements in each class
 
         cl=0 #counter for the classes, starting at 0
 
-        avg=0 #variable where the ratios of balls per number of elements of each class will be added, and later averaged
+        if(imb):
+            avg = np.zeros(len(self.classes))
+        else:
+            avg=0 #variable where the ratios of balls per number of elements of each class will be added, and later averaged
 
+         
         for cla in clas_dif: #for each class
 
             bolascla=0 #counter for the number of balls necessary for class coverage 
 
             falta = lista_el_cla[cl] #list of uncovered instances of that class, which initially includes all elements of said class
 
             while len(falta)!=0: #while there are uncovered elements of said class
@@ -2473,35 +2695,42 @@
                     bolas = [falta.index(i) for i in s[s].index.values] #said instances are saved as a list
 
                     if len(bolas) > len(bolaslist): #if this ball covers more instances than the previous best candidate
 
                         bolaslist = bolas #its covered elements are saved
 
                 bolascla+=1 #the total of chosen balls for the coverage of said class increases by 1
-
+                instance_per_ball.append(bolaslist)
                 for ele in sorted(bolaslist, reverse = True): 
 
                     del falta[ele] #the elements covered by chosen ball are deleted from the list of uncovered instances 
 
-            avg += (bolascla / el_cla[cl]) #the ratio between the number of balls necessary to cover the points of a class and the number of points of that class is added to the sum
+            if(imb):
+                avg[cl] = bolascla / el_cla[cl]
+            else:
+                avg += (bolascla / el_cla[cl]) #the ratio between the number of balls necessary to cover the points of a class and the number of points of that class is added to the sum
 
             cl+=1 #continue to the next class
-
-        return avg / len(clas_dif) #return the average of the ratios between the number of balls necessary to cover the points of a class and the number of points of that class
+        if(imb):
+            return avg
+        else:
+            return avg / len(clas_dif) #return the average of the ratios between the number of balls necessary to cover the points of a class and the number of points of that class
 
 
 
 
 
     def ONB_tot(self):
 
         """
 
         ONB complexity metric using the total number of balls
-
+        ------
+        Returns:
+        tot (float): The ratio between the number of balls necessary for full coverage and the number of instances of the dataset
     
         """
         
         featu = pd.DataFrame(self.X) #feature part of the dataframe
         
         clas = pd.DataFrame(self.y) #class part of the dataframe
```

### Comparing `pycol_complexity-0.0.5/pycol_complexity.egg-info/PKG-INFO` & `pycol_complexity-0.0.6/pycol_complexity.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycol_complexity
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python Package for complexity measures
 Home-page: https://github.com/DiogoApostolo/pycol
 Author: Diogo Apostolo
 Author-email: ogoid.478@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pycol_complexity-0.0.5/setup.cfg` & `pycol_complexity-0.0.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7963 6f6c 5f63 6f6d 706c 6578   = pycol_complex
 00000020: 6974 790d 0a76 6572 7369 6f6e 203d 2030  ity..version = 0
-00000030: 2e30 2e35 0d0a 6175 7468 6f72 203d 2044  .0.5..author = D
+00000030: 2e30 2e36 0d0a 6175 7468 6f72 203d 2044  .0.6..author = D
 00000040: 696f 676f 2041 706f 7374 6f6c 6f0d 0a61  iogo Apostolo..a
 00000050: 7574 686f 725f 656d 6169 6c20 3d20 6f67  uthor_email = og
 00000060: 6f69 642e 3437 3840 676d 6169 6c2e 636f  oid.478@gmail.co
 00000070: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
 00000080: 2050 7974 686f 6e20 5061 636b 6167 6520   Python Package 
 00000090: 666f 7220 636f 6d70 6c65 7869 7479 206d  for complexity m
 000000a0: 6561 7375 7265 730d 0a6c 6f6e 675f 6465  easures..long_de
```

