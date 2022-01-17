# [pandas.concat](https://pandas.pydata.org/docs/reference/api/pandas.concat.html)

## Example setup -1 Dataframe
- df1 = pd.DataFrame([['a', 1], ['b', 2]],
                   columns=['letter', 'number'])
![image](https://user-images.githubusercontent.com/49121293/149732239-bedf1b60-5f91-4159-a727-0c35f73ec945.png)
- df2 = pd.DataFrame([['c', 3], ['d', 4]],
                   columns=['letter', 'number'])
![image](https://user-images.githubusercontent.com/49121293/149732395-db89cd5f-9857-4611-a5d0-19dc541b9e3b.png)

- df3 = pd.DataFrame([['c', 3, 'cat'], ['d', 4, 'dog']],
                   columns=['letter', 'number', 'animal'])
![image](https://user-images.githubusercontent.com/49121293/149734015-5226d041-744b-4182-95ec-843f3691e845.png)


## parameters
### objs
- a sequence 
- mapping of Series
- DataFrame

#### Example : Combine two DataFrame objects with identical columns.

- pd.concat([df1, df2])
![image](https://user-images.githubusercontent.com/49121293/149732445-5cc9f069-35e1-4d70-941e-76897bfb840e.png)

### axis 
- 0 -> index (default)
- 1 -> columns





### ignore_index 
- False (default)
- True -> reset index.



### join
- inner
- outer -> default

#### Combine DataFrame objects with overlapping columns and return only those that are shared by passing inner to the join keyword argument.
![image](https://user-images.githubusercontent.com/49121293/149734916-05209f23-796f-4824-b66b-306c66846cf2.png)
![image](https://user-images.githubusercontent.com/49121293/149734995-4c53ddb6-6bec-44c9-83ee-f6e3445123e8.png)



