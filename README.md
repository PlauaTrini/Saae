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
    Fluoretos = float(input("Fluoretos(mg/l F):",))
    Dioxido_de_Carbono_Livre = float(input("Dióxido de Carbono Livre(mg/l CO2):",))
    Dureza_Total = float(input("Dureza Total (mg/l CaCO3):",))
    Nitratos = float(input("Nitratos(mg/l N):",))
    Nitritos = float(input("Nitritos(mg/l N):",))
    pH = float(input("pH(uT):",))
    def qualidade(): #fazer as análises#
        Cor_aparente = float(input("Cor Aparente(uH):",))
        if Cor_aparente>6.0:
            print ("Valor de cor aparente acima do Valor Máximo permitido, segundo a portaria nº 518 do Ministério da Saúde")
        turbidez=float(input("Turbidez(uT)::"))
        if turbidez>5.0:
            print ("Valor de turbidez acima do Valor Máximo permitido, segundo a portaria nº 518 do Ministério da Saúde")
        Acidez=float(input("Acidez(mg/l CO2):",))
        if Acidez>0.9:
            print ("Valor de acidez acima do Valor Máximo permitido, segundo a portaria nº 518 do Ministério da Saúde")
        Alcalinidade_Total =input("Alcalinidade Total(mg/l CaCO3):",)
        if Alcalinidade_Total>500.0:
            print ("Valor de alcalinidade acima do Valor Máximo permitido, segundo a portaria nº 518 do Ministério da Saúde")
        Aluminio = input("Aluminio(mg/l Al):",)
        if Aluminio>0.2:
            print ("Valor de aluminio acima do Valor Máximo permitido, segundo a portaria nº 518 do Ministério da Saúde")
        Amonia = float(input("Amonia(mg/l NH3):",))
        if Amonia>1.5:
            print ("Valor de amonia acima do Valor Máximo permitido, segundo a portaria nº 518 do Ministério da Saúde")
        Carbonato_de_Calcio = float(input("Carbonato de Cálcio(mg/l CaCO3):",))
        Cloro_Residual = float(input("Cloro Residual(mg/l Cl2):"))
        if Cloro_Residual>5.0:
            print ("Valor de cloro cesidual acima do Valor Máximo permitido, segundo a portaria nº 518 do Ministério da Saúde")
        Cloreto_Total = float(input("Cloreto Total(mg/l Cl):"))
        if Cloreto_Total>250.0:
            print ("Valor de cloreto total acima do Valor Máximo permitido, segundo a portaria nº 518 do Ministério da Saúde")
        Condutividade = float(input("Condutividade(Microsimens/em):",))
        Ferro_Total = float(input("Ferro Total(mg/l Fe):",))
        if Ferro_Total>0.3:
            print ("Valor de ferro total acima do Valor Máximo permitido, segundo a portaria nº 518 do Ministério da Saúde")
        Fluoretos = float(input("Fluoretos(mg/l F):",))
        if Fluoretos>1.5:
            print ("Valor de fluoretos acima do Valor Máximo permitido, segundo a portaria nº 518 do Ministério da Saúde")
        Dioxido_de_Carbono_Livre = float(input("Dióxido de Carbono Livre(mg/l CO2):",))
        if Dioxido_de_Carbono_Livre>500.0:
            print ("Valor de dioxido de carbono livre acima do Valor Máximo permitido, segundo a portaria nº 518 do Ministério da Saúde")
        Dureza_Total = float(input("Dureza Total (mg/l CaCO3):",))
        if Dureza_Total>500.0:
            print ("Valor de dureza total acima do Valor Máximo permitido, segundo a portaria nº 518 do Ministério da Saúde")
        Nitratos = float(input("Nitratos(mg/l N):",))
        if Nitratos>10.0:
            print ("Valor de nitratos acima do Valor Máximo permitido, segundo a portaria nº 518 do Ministério da Saúde")
        Nitritos = float(input("Nitritos(mg/l N):",))
        if Nitritos>1.0:
            print ("Valor de nitritos acima do Valor Máximo permitido, segundo a portaria nº 518 do Ministério da Saúde")
        pH = float(input("pH(uT):",))
        if 6<pH<9:
            print ("Valor de pH fora do intervalo permitido, segundo a portaria nº 518 do Ministério da Saúde")
        else:
        print("Escolha uma das opcoes abaixo:(digitando o seu codigo e apertando enter"))
        print("1.Voltar ao Menu Inicial                    2.Sair do programa")
        resposta = int(input())
        if RESPOSTA==1:
            menu_inicial()
    confirmar = input("Confirmar dados?(Sim ou não)")
    CONFIRMAR = confirmar.upper()
    if CONFIRMAR == "SIM":
        qualidade()
    else:
        print("Escolha uma das opções abaixo:(digitando o seu código e apertando enter)")
        print("1.Voltar ao Menu Inicial                    2.Sair do programa")
        resposta = int(input())
        if RESPOSTA==1:
            menu_inicial()

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
        print("Deseja realmente sair?(Sim ou não)")
        resposta2=input()
        resposta2.upper()
        if resposta2 != "SIM":
            print("Redirecionando para o menu inicial...")
            menu_inicial
Usuario = input("Usuário:",)
Senha = input("Senha:",)
if Usuario == "Martha Diva" and Senha == "euamocalculo":
    menu_inicial()
else:
    print ("Usuário e/ou senha inválidos")
