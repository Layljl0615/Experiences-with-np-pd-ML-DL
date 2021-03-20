1，torch.argmax()  -- Return specifies the sequence number of the maximum value of the dimension.
```
import torch
a=torch.tensor(
              [
                  [1, 5, 5, 2],
                  [9, -6, 2, 8],
                  [-3, 7, -9, 1]
              ])
b=torch.argmax(a,dim=0)
print(b)
print(a.shape)

# Result
tensor([1, 2, 0, 1])
torch.Size([3, 4])
```
2. df.shape  -- check the size of a dataframe.
```
def test():
        names = ['c1', 'c2', 'c3', 'c4', 'c5']
        df = pd.read_csv("testdata", sep="\t", header=None, names=names)
        print(df.info())
        print("\n")
        print("len is: ", len(df))
        print("columns is: ", df.columns)
        print("shape is: ", df.shape)
        print("size is: ", df.size)

# Result
<class 'pandas.core.frame.DataFrame'>
RangeIndex: 10 entries, 0 to 9
Data columns (total 5 columns):
 #   Column  Non-Null Count  Dtype
---  ------  --------------  -----
 0   c1      10 non-null     int64
 1   c2      10 non-null     int64
 2   c3      10 non-null     int64
 3   c4      10 non-null     int64
 4   c5      10 non-null     int64
dtypes: int64(5)
memory usage: 528.0 bytes
None


len is:  10
columns is:  Index(['c1', 'c2', 'c3', 'c4', 'c5'], dtype='object')
shape is:  (10, 5)
size is:  50

```
