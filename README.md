# palindrome_fun_string.py
#palindrome 
# A string is called palindrome if itreads same backwards as forward. 
#Forexample,
#Kanak is a palindrome.
#madam is a palindrome.
#function to check  if the string is palindrome or not 
def checkpalin(st):
    i=0
    j=len(st)-1
    while i<=j:
        if st[i]!=st[j]:
            return False
        i+=1
        j-=1
    return True
#function ends here
st=input("enter a string:")
#function calling
checkpalin(st)
result=checkpalin(st)
if result== True:
    print("the given string" ,st, "is a palindriome")
else:
    print("the given string ",st,"is not a palindrome")
