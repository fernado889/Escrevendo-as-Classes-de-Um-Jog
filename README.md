# Escrevendo-as-Classes-de-Um-Jog
class Heroi:
    def __init__(self, nome, idade, tipo):
        self.nome = nome
        self.idade = idade
        self.tipo = tipo

    def atacar(self):
        ataques = {
            "mago": "usou magia",
            "guerreiro": "usou espada",
            "monge": "usou artes marciais",
            "ninja": "usou shuriken"
        }

        ataque = ataques.get(self.tipo, "usou um ataque desconhecido")
        print(f"O {self.tipo} atacou usando {ataque}")


# Exemplo de uso
heroi1 = Heroi("Aragorn", 30, "guerreiro")
heroi1.atacar()

heroi2 = Heroi("Gandalf", 1000, "mago")
heroi2.atacar()

heroi3 = Heroi("Kung Fu", 25, "monge")
heroi3.atacar()

heroi4 = Heroi("Naruto", 20, "ninja")
heroi4.atacar()
O guerreiro atacou usando usou espada
O mago atacou usando usou magia
O monge atacou usando usou artes marciais
O ninja atacou usando usou shuriken
