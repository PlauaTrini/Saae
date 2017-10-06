#Definição de funções#
def inserir_dados():
    data = input("Insira a data (dd mm aaaa):").split()
    lista_data = []
    for i in range(len(data)):
        lista_data.append(int(data[i]))
    local = input("Insira o Local da Coleta:")
    print("Parâmetros Físicos")
    Cor_aparente = float(input("Cor Aparente(uH):",))
    turbidez=float(input("Turbidez(uT)::"))
    print("Parâmetros Químicos")
    Acidez=float(input("Acidez(mg/l CO2):",))
    Alcalinidade_Total =input("Alcalinidade Total(mg/l CaCO3):",)
    Aluminio = input("Aluminio(mg/l Al):",)
    Amonia = float(input("Amonia(mg/l NH3):",))
    Carbonato_de_Calcio = float(input("Carbonato de Cálcio(mg/l CaCO3):",))
    Cloro_Residual = float(input("Cloro Residual(mg/l Cl2):"))
    Cloreto_Total = float(input("Cloreto Total(mg/l Cl):"))
    Condutividade = float(input("Condutividade(Microsimens/em):",))
    Ferro_Total = float(input("Ferro Total(mg/l Fe):",))
    Fuoretos = float(input("Fluoretos(mg/l F):",))
    Dioxido_de_Carbono_Livre = float(input("Dióxido de Carbono Livre(mg/l CO2):",))
    Dureza_Total = float(input("Dureza Total (mg/l CaCO3):",))
    Nitratos = float(input("Nitratos(mg/l N):",))
    Nitritos = float(input("Nitritos(mg/l N):",))
    pH = float(input("pH(uT):",))
    def qualidade(): #fazer as análises#
        Cor_aparente = float(input("Cor Aparente(uH):",))
        turbidez=float(input("Turbidez(uT)::"))
        Acidez=float(input("Acidez(mg/l CO2):",))
        Alcalinidade_Total =input("Alcalinidade Total(mg/l CaCO3):",)
        Aluminio = input("Aluminio(mg/l Al):",)
        Amonia = float(input("Amonia(mg/l NH3):",))
        Carbonato_de_Calcio = float(input("Carbonato de Cálcio(mg/l CaCO3):",))
        Cloro_Residual = float(input("Cloro Residual(mg/l Cl2):"))
        Cloreto_Total = float(input("Cloreto Total(mg/l Cl):"))
        Condutividade = float(input("Condutividade(Microsimens/em):",))
        Ferro_Total = float(input("Ferro Total(mg/l Fe):",))
        Fuoretos = float(input("Fluoretos(mg/l F):",))
        Dioxido_de_Carbono_Livre = float(input("Dióxido de Carbono Livre(mg/l CO2):",))
        Dureza_Total = float(input("Dureza Total (mg/l CaCO3):",))
        Nitratos = float(input("Nitratos(mg/l N):",))
        Nitritos = float(input("Nitritos(mg/l N):",))
        pH = float(input("pH(uT):",))
    confirmar = input("Confirmar dados?")
    CONFIRMAR = confirmar.upper()
    if CONFIRMAR == "SIM":
        arquivo={}
        arquivo["DATA"] = lista_data
        arquivo["LOCAL"]=local
        arquivo["TEMPERATURA"]=temperatura
        arquivo["COR"]=cor
        arquivo["ODOR"]=odor
        arquivo["TURBIDEZ"]=turbidez
        arquivo["PH"]=ph
        arquivo["OD"]=od
        arquivo["DBO"]=dbo
        arquivo["DQO"]=dqo
        arquivo["COLIFORMES"]=coliformes
        print(arquivo)
        return None
    else:
        print("Voltar para o menu inicial?")
        resposta = input()
        RESPOSTA = resposta.upper()
        if RESPOSTA=="SIM":
            return None
        else:
            inserir_dados()

def consultar_banco():
    print("Em Construção")
def corrigir_dados():
    print("Em Construção")
def estatisticas():
    print("Em Construção")
def cadastrar_usuario():
    print("Em Construção")

#Menu inicial#
def menu_inicial():
    print("Escolha uma das opções abaixo:(digitando o seu código e apertando enter)")
    print("1.Inserir Dados                    2.Consultar Banco de Dados")
    print("3.Atualizar/Corrigir Dados         4.Estatísticas")
    print("5.Cadastrar Usuário                6.Sair")
    resposta = int(input())
    if resposta == 1:
        inserir_dados()
    elif resposta == 2:
        consultar_banco()
    elif resposta == 3:
        corrigir_dados()
    elif resposta == 4:
        estatisticas()
    elif resposta == 5:
        cadastrar_usuario()
    elif resposta == 6:
        print("Deseja realmente sair?")
        resposta2=input()
Usuario = input("Usuário:",)
Senha = input("Senha:",)
if Usuario == "Martha Diva" and Senha == "euamocalculo":
    menu_inicial()
else:
    print ("Usuário e/ou senha inválidos")
