# project01

[projeto01.py](https://github.com/user-attachments/files/25223919/projeto01.py)
compras = []

while True:
   
    print('\n1 - adicionar item a lista ')
    print('2 - mostrar item como comprado ')
    print('3 - mostrar lista ')
     
    opcao = input('digite qual você deseja escolher: ')
    
    if opcao == '1':
        item = input('adicione um item:')
        compras.append([item, False])
        print('\nitem adicionado com sucesso')
    
    elif opcao == '2':
        print('\nSUA LISTA: ')
        for i in range(len(compras)):
            status = '✔' if compras [i][1] else '✘'
            print(f'{i} - {compras[i][0]} [{status}]')
        
        num = int(input('digite o numero do item comprado: '))
        compras[num][1] = True
        print('item marcado como comprado! ')
   
    elif opcao == '3':
        print('\nsua lista: ')
        for item in compras:
            status = '✔' if  item[1] else '✘'
            print (f'- {item[0]} [{status}]')
         
          
    
    
