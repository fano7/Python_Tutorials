# simple Decision Tree Classifier

/badge/dynamic/json.svg?url=<URL>&label=<LABEL>&query=<$.DATA.SUBDATA>&colorB=<COLOR>&prefix=<PREFIX>&suffix=<SUFFIX>



```python



from sklearn import tree

D3 = tree.DecisionTreeClassifier()


X = [
    [177,10,0.3 ], #man
    [175, 42,0.7],    # woman                                                          
      [136, 35,0.6],    # woman                                                         
      [174, 15,0.1],     # man                                                         
      [141, 28,0.8]     # woman ]
]


Y = [
    'man',
    'woman',
     'woman',
     'man', 
     'woman'
]


D3 = D3.fit(X,Y)


prediction = D3.predict ( [ [177 , 40 , 0.4 ] ])
print( prediction )
