# merge two data frames in pyspark
If you are creating two data frames from two different sources which have same columns but in different order,  pyspark will not allow to merge these data frames.First make sure both the data frames have same order of colums and then merge.  
`df1 = df1.select(sorted(df1.columns))`  
`df2 = df2.select(sorted(df2.columns))`  
`df3 = df1.union(df2)`  
  
  Here df1.colums and df2.colums have the same columns (may be in different order)

