1，torch.argmax()  #Return specifies the sequence number of the maximum value of the dimension
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
