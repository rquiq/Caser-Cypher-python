#dev by: younse raquiq
#v1.0

#chose crypt() or dcrypt()


def crypt():
    alphabet = 'abcdefghijklmnopqrstuvwxyz' 
    key = int(input('Enter a key : '))
    Nmessage = ''

    fileName = input('Enter a file name : ')
    message = open(fileName).read()

    for ch in message:
        if ch in alphabet:
            position = alphabet.find(ch)
            Nposition = (position + key )%26
            Nch = alphabet[Nposition]

            Nmessage += Nch
        else:
            Nmessage += ch

    print(Nmessage)
    file = open(fileName,'w')
    file.write(Nmessage)
    file.close()

def dcrypt():
    alphabet = 'abcdefghijklmnopqrstuvwxyz'
    key = int(input('Enter a key : '))
    Nmessage = ''

    fileName = input('Enter a file name : ')
    message = open(fileName).read()

    for ch in message:
        if ch in alphabet:
            position = alphabet.find(ch)
            Nposition = (position - key )%26
            Nch = alphabet[Nposition]

            Nmessage += Nch
        else:
            Nmessage += ch

    print(Nmessage)
    file = open(fileName,'w')
    file.write(Nmessage)
    file.close()
