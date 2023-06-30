# Lista de Lanchonetes

Lista de lanchonetes de qualquer lugar do mundo com informação compartilhada no github.

## Objetivo

Esta lista pretende ser uma lista com fins didáticos porém práticos. A lista contém dados reais de estabelecimentos que fornecem comida. Pode ser lanchonete, restaurante, barraca de feira, carrocinha de calçada, vendedor ambulante, pizzaria, temakeria, churrascaria, padaria, frango no espeto, marmiteira, sorveteria, whatever

A ideia é utilizar os comandos git para permitir que a atualização da lista seja pública e compartilhada, demonstrando os conceitos de compartilhamento de código (no caso texto), versionamento, controle de alterações (pull requests), edição descentralizada e concorrente com múltiplos colaboradores.

Além de servir para demonstrar os comandos git utilizados para manter código remotamente, essa lista pode quebrar um galhão dando dicas sobre locais com boa comida e que não são lá muito formais. Em algumas cidades, acontece da melhor comida ser feita informalmente.

## Formato

A lista é formatada em JSON com alguns campos básicos fundamentais descritos a seguir

-nome : nome do estabelecimento, como é conhecido
-tipo : lanchonete, churrascaria, padaria, vendinha, ambulante, restaurante, sorveteria, bodega, espelunca, carrocinha, trailer, foodtruck, marmiteira, whatever
-endereco : Local onde fica o estabelecimento. A ideia aqui é dar a dica de como chegar lá
-cidade : cidade onde fica o estabelecimento
-estado : estado onde fica o estabelecimento
-apps : lista dos aplicativos em que se pode fazer o pedido. Tipo, Ifood, zédelivery, rangobom, etc. Pode ser vazia
-site : é o site do estabelecimento na internet, se houver
-fone : é o telefone para falar com o estabelecimento
-whatsapp: é o whatsapp para falar e fazer pedidos, se houver.

Os campos nome, tipo, endereco, cidade, estado e fone são obrigatórios. Os outros campos são opcionais. Se quiserem adicionar campos a lista podem adicionar. Coisas como "formas de pagamento", "coordenadas gps", "horário de funcionamento", "fechou/faliu", "prato recomendado", "dica para chegar", usem a imaginação.

## Como colaborar

Qualquer pessoa pode colaborar com a edição da lista. Se você conhece algum lugar legal com uma boa comida e quer compartilhar, faça um clone desse repositório, crie uma branch, edite o arquivo lista-lanchonetes.json, dê um push e em seguida crie um pull request.

Todos os PR's serão analisados pelos colaboradores habilitados e o PR será aceito ou rejeitado. Todas as contribuições são bem vindas.

## Sequência de comandos

```bash
# copia a lista para o comptuador local
git pull git@github.com:Bokomoko/lista-de-lanchonetes.git
# cria uma branch com um nome qualquer
git checkout -b <nomeQueVocêQuiserParaSuaBranch>
# ... edit o arquivo lista-lanchonetes.json usando o editor que quiser
git add lista-lanchonetes.json
git commit -m <coloque aqui uma mensagem sobre a alteração que fez>
git push
```

Após completar o push, vá ao site do [repositório no Github](<https://github.com/Bokomoko/lista-de-lanchonetes>) e crie um pull request. agora é só esperar que em tempo a sua contribuição será adicionada
