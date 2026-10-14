<!DOCTYPE html>
<html lang="pt">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Escola Presença Online</title>

    <link rel="stylesheet" href="style.css">
</head>

<body>

    <!-- CABEÇALHO -->
    <header>
        <div class="logo">
            🎓 Escola <span>Presença Online</span>
        </div>

        <nav>
            <a href="#inicio">Início</a>
            <a href="#sobre">Sobre</a>
            <a href="#servicos">Serviços</a>
            <a href="#avisos">Avisos</a>
            <a href="#contactos">Contactos</a>
        </nav>
    </header>

    <!-- APRESENTAÇÃO -->
    <section id="inicio" class="hero">
        <div class="hero-content">
            <h1>Bem-vindo à Escola<br>
                <span>Presença Online</span>
            </h1>

            <p>
                Uma plataforma digital criada para aproximar
                alunos, professores, encarregados de educação
                e a direção da escola.
            </p>

            <a href="#servicos" class="botao">
                Explorar plataforma
            </a>
        </div>
    </section>

    <!-- SOBRE -->
    <section id="sobre" class="secao">
        <h2>Sobre o Programa</h2>

        <p>
            A Escola Presença Online é um projeto que pretende
            facilitar o acesso à informação escolar através
            da internet.

            A plataforma permite divulgar informações,
            consultar horários, acompanhar notas e melhorar
            a comunicação entre a escola e os alunos.
        </p>
    </section>

    <!-- SERVIÇOS -->
    <section id="servicos" class="secao">
        <h2>O que podes fazer?</h2>

        <div class="cartoes">

            <div class="cartao">
                <div class="icone">📊</div>
                <h3>Consultar Notas</h3>
                <p>
                    Acompanha o teu desempenho académico
                    e consulta as tuas classificações.
                </p>
                <button onclick="abrirServico('notas')">
                    Consultar
                </button>
            </div>

            <div class="cartao">
                <div class="icone">📅</div>
                <h3>Horários</h3>
                <p>
                    Consulta os horários das aulas
                    e organiza melhor o teu tempo.
                </p>
                <button onclick="abrirServico('horarios')">
                    Ver horários
                </button>
            </div>

            <div class="cartao">
                <div class="icone">📢</div>
                <h3>Avisos</h3>
                <p>
                    Descobre os comunicados, eventos
                    e informações importantes da escola.
                </p>
                <button onclick="abrirServico('avisos')">
                    Ver avisos
                </button>
            </div>

            <div class="cartao">
                <div class="icone">📝</div>
                <h3>Trabalhos</h3>
                <p>
                    Consulta as orientações para trabalhos
                    e atividades escolares.
                </p>
                <button onclick="abrirServico('trabalhos')">
                    Saber mais
                </button>
            </div>

            <div class="cartao">
                <div class="icone">👨‍🏫</div>
                <h3>Professores</h3>
                <p>
                    Facilita a comunicação entre
                    professores e alunos.
                </p>
                <button onclick="abrirServico('professores')">
                    Saber mais
                </button>
            </div>

            <div class="cartao">
                <div class="icone">🔐</div>
                <h3>Acesso ao Sistema</h3>
                <p>
                    Área destinada aos utilizadores
                    autorizados da plataforma.
                </p>
                <button onclick="mostrarLogin()">
                    Entrar
                </button>
            </div>

        </div>
    </section>

    <!-- ÁREA DE CONTEÚDO DINÂMICO -->
    <section id="area-dinamica" class="secao" hidden>
        <h2 id="titulo-dinamico"></h2>
        <div id="conteudo-dinamico"></div>

        <button onclick="fecharServico()" class="botao">
            Fechar
        </button>
    </section>

    <!-- FORMULÁRIO DE ACESSO -->
    <section id="login" class="secao" hidden>
        <h2>Acesso à Plataforma</h2>

        <p>
            Introduz os teus dados de acesso autorizados.
        </p>

        <form id="form-login">
            <label for="utilizador">Utilizador ou e-mail</label>

            <input
                type="text"
                id="utilizador"
                placeholder="O teu utilizador"
                required
            >

            <label for="senha">Palavra-passe</label>

            <input
                type="password"
                id="senha"
                placeholder="A tua palavra-passe"
                required
            >

            <button type="submit" class="botao">
                Entrar
            </button>

            <p id="mensagem-login" aria-live="polite"></p>
        </form>
    </section>

    <!-- AVISOS -->
    <section id="avisos" class="secao">
        <h2>Informações da Escola</h2>

        <div class="aviso">
            <h3>📢 Comunicados escolares</h3>
            <p>
                Consulta nesta área os comunicados oficiais
                publicados pela direção da escola.
            </p>
        </div>

        <div class="aviso">
            <h3>📅 Calendário académico</h3>
            <p>
                Consulta as datas de avaliações,
                reuniões e outras atividades escolares.
            </p>
        </div>
    </section>

    <!-- CONTACTOS -->
    <section id="contactos" class="secao">
        <h2>Contacta a Escola</h2>

        <p>
            Para informações, dúvidas ou apoio,
            entra em contacto com a secretaria da escola.
        </p>

        <p>📧 E-mail: contacto@escola.com</p>
        <p>📞 Telefone: +000 000 000 000</p>
        <p>📍 Endereço: inserir endereço da escola</p>
    </section>

    <!-- RODAPÉ -->
    <footer>
        <h3>🎓 Escola Presença Online</h3>

        <p>
            Tecnologia ao serviço da educação.
        </p>

        <p>
            &copy; <span id="ano"></span>
            Escola Presença Online.
            Todos os direitos reservados.
        </p>
    </footer>

    <script src="script.js"></script>

</body>
</html>
