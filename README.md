fname=input('Enter file directory/name: ')
c=[]
d={}
with open(fname,'r') as f:
content=f.read()
word=content.split()
for i in word:
c.append(i)
for i in c:
count=0
for j in c:
if i==j:
count+=1
d[i]=count
sortd=sorted(d.items(), key=lambda x:x[1], reverse=True)
print(sortd[0:10])





fname=input('Enter file name/directory: ')
with open(fname,'r') as f:
read=f.read()
word=read.split()
l=[]
for i in word:
l.append(i)
l.sort()
wname=input('Enter file name to create: ')
with open(wname,'w') as w:
for j in l:
w.write(j)
w.write('\n')
OUTPUT
