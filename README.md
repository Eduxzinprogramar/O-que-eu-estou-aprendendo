enum Cor { Azul, Verde, Amarelo, Vermelho }
enum Opcao { Criar = 1, Deletar, Editar, Listar, Atualizar }

static void Main(string[] args)
{
    Console.WriteLine("Selecione uma das opções abaixo: ");
    Console.WriteLine("1-Criar\n2-Deletar\n3-Editar\n4-Listar\n5-Atualizar");
    int index = int.Parse(Console.ReadLine());
    Opcao opcaoSelecionada = (Opcao)index;

    switch (opcaoSelecionada)
    {
        case Opcao.Criar:
            Console.WriteLine("Você quer criar algo!");
            break;
        case Opcao.Deletar:
            Console.WriteLine("Você quer deletar este item!");
            break;
        case Opcao.Editar:
            Console.WriteLine("Você gostaria de editar esse item");
            break;
    }
