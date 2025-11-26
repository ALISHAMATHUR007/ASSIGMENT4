
f=open("sample.txt","w")
f.write("ine1:this is a simple text file.\n")
f.write("line2:it contains multiple lines.")
f.write('bye')
f.close()
print("work is done")

try:
    with open("sample.txt", "r") as file:
        content = file.read()
        print(content)
except FileNotFoundError:
    print("Error: The file 'sample.txt' does not exist.")


