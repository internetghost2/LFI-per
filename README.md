# LFI-per


#python
dot = ""
dic = ["home", "hola", "dsdas", "prova", "dsakdsads", "dsadadasdsa", "1", "8"]

num = 0
#per que faci fins al final de la llista
num1 = (len(dic)) - 1



for i in range(10):
    num = 0
    dots = ""
    dot = dot + "../"
    dic1 = dic[num]
    dots = dot + str(dic1) + "/flag.txt"
    flag = dot + "flag.txt"  
    print (flag)
    
    while num <=num1:
        
        print (dots)
        num = num + 1
