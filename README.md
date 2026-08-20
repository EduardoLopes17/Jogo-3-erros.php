1- Descrição dos Problemas Encontrados

Analisando o código linha por linha, encontrei 3 erros de sintaxe e execução e 1 falha de segurança.

Erros de Sintaxe:

1- Erro: "$stmt->bind_param("ssi", $nome, $email, $id)"
2- Erro: "$resultado = $conn->query($sql)"
3- Erro: "die("Erro na conexão: " . $conn->connect_error)"

2- A Falha de Segurança:

Falha de Segurança: Remoção via GET sem confirmação 
O botão de excluir é um link do tipo GET (<a href="index.php?excluir=1">Excluir</a>).

Erros:

<a href="index.php?excluir=...">Excluir</a>
if (isset($_GET['excluir']))