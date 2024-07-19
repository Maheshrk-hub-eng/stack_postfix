a=input()
s=[]
for i in range (len(a)):
    if a[i]>='0' and a[i]<='9':
        s.append(int(a[i]))
    else:
        v1=s.pop()
        v2=s.pop()
        if a[i]=='+':
            s.append(v2+v1)
        elif a[i]=='-':
            s.append(v2-v1)
        elif a[i]=='*':
            s.append(v2*v1)
        elif a[i]=='/':
            s.append(v2//v1)
print(int(*s))
