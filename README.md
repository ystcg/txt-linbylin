file=open("rhyme.txt","w")
file.write('''would it be ok if i took some of your time?
would it be ok if i wrote you a rhyme?''')
file.close()

file=open("rhyme.txt")
lines=file.readlines()
for line in lines:
    words=line.split()
    for word in words:
        print(word+'#',end='')
    print()
file.close()
