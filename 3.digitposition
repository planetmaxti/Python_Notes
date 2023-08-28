def main():
    print("hey there")

    #rango de buscqueda
    rbus = 999999
    condi = False
    for x in range(142852,rbus,1):
        
        #condicional para parar si lo encuentra:
        if(condi == True):
            print('Lo encontramos')
            break
        else:
            #Num in array form.
            print('***{}'.format(x+1))
            digits = dig(x+1)
            #print('Los digitos son:{0}'.format(digits))
            #New position
            reposition = newnum(digits)
            #Nevo arreglo en el nuevo orden
            arraydigit = reposition[2]
            #Prueba del tamaño del arreglo y si es el numero correcto
            #print('Length of innitial array:{0}, length new array:{1}'.format(reposition[0], reposition[1]))
            #print('Nuevo numero es:{}'.format(arraydigit))
            unido = union(arraydigit)
            print(unido)
            print(prueba(x+1, unido))
            #verificacion si ya lo encontro
            precondi = prueba(x+1, unido)
            condi = precondi[0]
            print(condi)



def dig(number):
    list_of_digits = []
    list_of_digits = list(map(int, str(number)))
    return list_of_digits

def newnum(arr):
    current_len = len(arr)
    new_index = 0
    element = arr.pop(current_len-1)
    arr.insert(new_index, element)
    new_len = len(arr)
    #print(arr)
    return (current_len, new_len, arr)


def union(arr2):

    numero = 0
    count = 0
    for element in reversed(arr2):
        numero = numero + element*10**count
        #prueba que el numero fue bien escrito
        #print('la cuenta es:', count)
        #print('el numero es:', numero)
        count = count + 1
    return numero

def prueba(num1, num2):
    a = 5
    puerta = False
    porcent = 0
    porcent = num2/num1
    if( num2 == num1*a ):
        print('ok')
        puerta = True
    else:
        print('.')

    return puerta, porcent

if __name__=="__main__":
    main()