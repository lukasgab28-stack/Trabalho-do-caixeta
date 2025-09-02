<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Git e GitHub - Guia Básico</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Lucida Grande', 'Bitstream Vera Sans', 'Helvetica Neue', sans-serif;
        }
        
        body {
            background-color: #f5f5f5;
            color: #333;
            line-height: 1.6;
            padding: 20px;
            max-width: 1000px;
            margin: 0 auto;
        }
        
        /* Cabeçalho no estilo Redmine */
        header {
            background-color: #9d261d;
            color: white;
            padding: 15px 20px;
            margin-bottom: 20px;
            border-radius: 3px;
            box-shadow: 0 1px 3px rgba(0, 0, 0, 0.2);
        }
        
        h1 {
            font-size: 20px;
            font-weight: bold;
        }
        
        /* Títulos no estilo Redmine */
        h2 {
            color: #9d261d;
            margin: 25px 0 15px;
            padding-bottom: 5px;
            border-bottom: 1px solid #e6e6e6;
            font-size: 16px;
            font-weight: bold;
        }
        
        /* Container principal */
        .container {
            background: white;
            border: 1px solid #e6e6e6;
            border-radius: 3px;
            padding: 0;
            overflow: hidden;
        }
        
        /* Conteúdo interno */
        .content {
            padding: 20px;
        }
        
        /* Estilo das caixas de informação */
        .box {
            background: #f8f8f8;
            border: 1px solid #e6e6e6;
            border-left: 3px solid #9d261d;
            padding: 15px;
            margin-bottom: 15px;
            border-radius: 2px;
        }
        
        /* Lista de comandos */
        .code-block {
            background: #2c2c2c;
            color: #f0f0f0;
            padding: 12px;
            margin: 10px 0;
            border-radius: 3px;
            font-family: monospace;
            font-size: 13px;
            overflow-x: auto;
        }
        
        /* Lista numerada */
        ol {
            margin-left: 20px;
            margin-bottom: 15px;
        }
        
        li {
            margin-bottom: 8px;
            padding-left: 5px;
        }
        
        /* Rodapé no estilo Redmine */
        footer {
            text-align: center;
            margin-top: 30px;
            padding: 15px;
            background: #f5f5f5;
            color: #555;
            border-top: 1px solid #e6e6e6;
            font-size: 12px;
        }
        
        /* Links */
        a {
            color: #9d261d;
            text-decoration: none;
        }
        
        a:hover {
            text-decoration: underline;
        }
        
        /* Tabela de diferenças */
        table {
            width: 100%;
            border-collapse: collapse;
            margin: 15px 0;
        }
        
        th, td {
            padding: 8px 12px;
            text-align: left;
            border: 1px solid #e6e6e6;
        }
        
        th {
            background-color: #f8f8f8;
            color: #9d261d;
        }
        
        tr:nth-child(even) {
            background-color: #f8f8f8;
        }
    </style>
</head>
<body>
    <header>
        <h1>Git e GitHub - Comandos Linux e Comandos GIT</h1>
    </header>
    
    <div class="container">
        <div class="content">
            <h2>O que é o Git</h2>
            <div class="box">
                <p>Git é um sistema de controle de versão distribuído de código aberto usado para rastrear alterações em qualquer conjunto de arquivos. Foi projetado para coordenar o trabalho entre programadores, mas pode ser usado para rastrear alterações em qualquer conjunto de arquivos.</p>
            </div>
            
            <h2>O que é o GitHub</h2>
            <div class="box">
                <p>GitHub é uma plataforma de hospedagem de código-fonte e arquivos com controle de versão usando o Git. Ele permite que programadores, utilitários ou qualquer usuário cadastrado na plataforma contribuam em projetos privados e/ou Open Source de qualquer lugar do mundo.</p>
            </div>
            
            <h2>Diferenças entre Git e GitHub</h2>
            <table>
                <tr>
                    <th>Git</th>
                    <th>GitHub</th>
                </tr>
                <tr>
                    <td>Software de controle de versão</td>
                    <td>Plataforma de hospedagem de código</td>
                </tr>
                <tr>
                    <td>Instalado localmente na máquina</td>
                    <td>Serviço baseado na nuvem</td>
                </tr>
                <tr>
                    <td>Focado no controle de versão</td>
                    <td>Adiciona recursos de colaboração</td>
                </tr>
                <tr>
                    <td>Não requer internet para uso básico</td>
                    <td>Requier internet para a maioria das operações</td>
                </tr>
            </table>
            
            <h2>Principais comandos Linux para Git Bash</h2>
            <div class="code-block">
                ls          # Listar arquivos e diretórios<br>
                cd          # Navegar entre diretórios<br>
                pwd         # Mostrar diretório atual<br>
                mkdir       # Criar diretório<br>
                rm          # Remover arquivo<br>
                cp          # Copiar arquivo<br>
                mv          # Mover ou renomear arquivo<br>
                cat         # Exibir conteúdo do arquivo<br>
                touch       # Criar arquivo vazio
            </div>
            
            <h2>Principais comandos Git</h2>
            <div class="code-block">
                git init                    # Inicializar repositório<br>
                git clone [url]             # Clonar repositório remoto<br>
                git add [arquivo]           # Adicionar arquivo ao staging<br>
                git commit -m "mensagem"    # Criar commit<br>
                git status                  # Verificar status<br>
                git push                    # Enviar para repositório remoto<br>
                git pull                    # Atualizar repositório local<br>
                git branch                  # Gerenciar branches<br>
                git checkout [branch]       # Alternar entre branches<br>
                git merge [branch]          # Mesclar branches
            </div>
            
            <h2>Como criar um repositório no GitHub</h2>
            <ol>
                <li>Faça login na sua conta GitHub</li>
                <li>Clique no botão "+" no canto superior direito</li>
                <li>Selecione "New repository"</li>
                <li>Digite um nome para o repositório</li>
                <li>Adicione uma descrição (opcional)</li>
                <li>Escolha entre repositório público ou privado</li>
                <li>Marque "Initialize this repository with a README" (opcional)</li>
                <li>Clique em "Create repository"</li>
            </ol>
            
            <h2>Como ligar um projeto existente ao GitHub</h2>
            <ol>
                <li>Crie um novo repositório no GitHub (sem README)</li>
                <li>Abra o terminal na pasta do projeto</li>
                <li>Execute: <span class="code-block" style="display: inline; padding: 2px 5px;">git init</span></li>
                <li>Execute: <span class="code-block" style="display: inline; padding: 2px 5px;">git add .</span></li>
                <li>Execute: <span class="code-block" style="display: inline; padding: 2px 5px;">git commit -m "primeiro commit"</span></li>
                <li>Execute: <span class="code-block" style="display: inline; padding: 2px 5px;">git branch -M main</span></li>
                <li>Execute: <span class="code-block" style="display: inline; padding: 2px 5px;">git remote add origin [URL_DO_REPOSITORIO]</span></li>
                <li>Execute: <span class="code-block" style="display: inline; padding: 2px 5px;">git push -u origin main</span></li>
            </ol>
            
            <h2>Como gerar uma versão com Git</h2>
            <ol>
                <li>Faça alterações nos arquivos do projeto</li>
                <li>Use <span class="code-block" style="display: inline; padding: 2px 5px;">git add [arquivo]</span> ou <span class="code-block" style="display: inline; padding: 2px 5px;">git add .</span></li>
                <li>Execute <span class="code-block" style="display: inline; padding: 2px 5px;">git commit -m "Mensagem descritiva"</span></li>
            </ol>
            
            <h2>Como enviar para o GitHub</h2>
            <ol>
                <li>Certifique-se de ter feito commit das alterações</li>
                <li>Execute <span class="code-block" style="display: inline; padding: 2px 5px;">git push origin [nome-da-branch]</span></li>
                <li>Se for a primeira vez, use <span class="code-block" style="display: inline; padding: 2px 5px;">git push -u origin [nome-da-branch]</span></li>
            </ol>
        </div>
    </div>
    
    <footer>
        <p>Desenvolvido por <strong>Seu Nome Completo</strong> | Entregue em: <strong>Data de Entrega</strong></p>
    </footer>
</body>
</html>
