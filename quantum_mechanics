import numpy as np

def degeneracy(num):
	s = 0
	x = (np.arange(num))+1
	[u,v] = np.meshgrid(x,x)
	n_ = u**2 + v**2
	for i in range(num):
		for j in range(num):
			t = np.where(n_==n_[i,j])
			if len(t[0]) > 2:
				# print(t)
				s = s + 1/len(t[0])
	return s

num = 100
s = degeneracy(num)
print(s)
