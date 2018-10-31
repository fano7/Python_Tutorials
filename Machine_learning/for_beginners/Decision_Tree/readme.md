# simple Decision Tree Classifier

```python



from sklearn import tree


# In[2]:


D3 = tree.DecisionTreeClassifier()


# In[3]:


X = [
    [177,10,0.3 ], #man
    [175, 42,0.7],    # woman                                                          
      [136, 35,0.6],    # woman                                                         
      [174, 15,0.1],     # man                                                         
      [141, 28,0.8]     # woman ]
]


# In[4]:


Y = [
    'man',
    'woman',
     'woman',
     'man', 
     'woman'
]


# In[5]:


D3 = D3.fit(X,Y)


# In[6]:


prediction = D3.predict ( [ [177 , 40 , 0.4 ] ])
print( prediction )


# In[7]:


prediction = D3.predict ( [ [135 , 29 , 0.8] ])
print( prediction )


# In[8]:


prediction = D3.predict ( [ [177 , 3 , 0 ] ])
print( prediction )


# In[9]:


prediction = D3.predict ( [ [144 , 50 , 1 ] ])
print( prediction )


# In[10]:


prediction = D3.predict ( [ [130 , 15 , 0.9 ] ])
print( prediction )


# In[11]:


prediction = D3.predict ( [ [130 , 4 , 0 ] ])
print( prediction )


```
