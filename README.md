print("bem vindo ao informações de alimentos!")

alimentos = ["Banana", "Maçã", "Laranja", "Abacaxi", "Melancia", "Pera", "Uva", "Manga", "Caju", "Kiwi"]
informacoes = {
    "banaana": "rica em potássio.",
    "maçã": "muito boa em fibras.",
    "laranja": "rica em vitamina C.",
    "abacaxi": "boa em digestão.",
    "melancia": "hidratante e rica em vitaminas A e C."
}

while True:
    escolha = input("Escolha um alimento ou 'sair' para terminar: ").lower()
    if escolha == "sair": break
    if escolha.capitalize() in alimentos:
        alimento = escolha.capitalize()
        print(f"Informações sobre {alimento}: {informacoes.get(alimento.lower(), 'Sem descrição disponível.')}")
    else:
        print("Alimento não encontrado.")
print("Ok, até a próxima!")
