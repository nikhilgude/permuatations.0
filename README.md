# permuatations.0
#permuatations of char in tree recursion
def permute(s, bucket=' '):
    if not s:
        print(bucket)
        return
    for i in range(len(s)):
        ns=s[:i]+s[i+1:]
        permute(ns,bucket+s[i])
text = input("enter a name/word: ")
print("possibilities of combinations.......")
permute(text)
