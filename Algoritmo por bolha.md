# meu-portfolio.py
Algoritmo de ordenação por bolhas
def bubble_sort(a_list): # a_list é a lista que será ordenada
    list_length = len(a_list) # Calcula o tamanho da lista
    for i in range(list_length - 1, 0, -1):# Loop externo que percorre a lista de trás para frente
        for j in range(i):# Loop interno que percorre a lista até o índice i
            if a_list[j] > a_list[j + 1]:# Compara o elemento atual com o próximo elemento
                a_list[j], a_list[j + 1] = a_list[j + 1], a_list[j]# Se o elemento atual for maior que o próximo, troca os elementos de posição
    return a_list
print(bubble_sort([5, 2, 9, 1, 4, 6, 3, 8, 7])) #Chama a função bubble_sort com uma lista de números e imprime a lista ordenada
