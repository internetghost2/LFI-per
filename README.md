# LFI-custom

Python 3

    print("Quin ...?")
    pregunta = input()
    file = open (pregunta, "a")
    dot = ""
    # directoris que vull, seran substiuits per un arxiu extern
    dic = ["directori1", "directori2", "directori3", "directori4", "directori5", "directori6", "directori7", "directori8"]
    #per que faci fins al final de la llista
    num1 = (len(dic)) - 1
    txt = "flag.txt"
    # bucle for i quantes vegades vull que es repateixi
    for i in range(10):
        #ens servira per indicar quina paraula de la llista dic volem agafar
        num = 0
        flag = dot + txt 
        print (flag)
        #afegim /.. cada vegada que passi.
        dot = dot + "../"

        #fem el bucle while per ampliar el numero que ha de buscar la llista 
        # significa que sempre que el valor que trobem dins num sigui més petit que num1 segeixi.
        while num <=num1:
            dic1 = dic[num]
            dots = dot + str(dic1) + "/" + txt
            print (dots)
            file.write(dots)
            num = num + 1
    file.close()
