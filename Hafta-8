from random import  randint


def createTable(size):
    hashTable = []
    for i in range(size):
        hashTable.append(0)
    print(hashTable)

    return hashTable


def myHash(numberToBeInserted, size):
    return numberToBeInserted % size


def insertMyHashTable(numberToBeInserted, myTable):
    isCollision = False
    index = myHash(numberToBeInserted, len(myTable))

    if (myTable[index] == 1):
        isCollision = True
    else:
        myTable[index] = 1

    return isCollision


def myTest(size , numberOfInsert):
    m_h_1 = createTable(size)
    c = 0
    for s in range(numberOfInsert):
        number = randint(0,1000)
        if(insertMyHashTable(number, m_h_1) == True):
            c += 1
    return c

myTable = createTable(13)

insertMyHashTable(26, myTable)
print(myTable)
print(myTest(23,20))
