<div align="center">
  <h1>📱 Presence+</h1>
  <p><strong>Frontend desenvolvido com Flutter & Dart</strong></p>
  
  <img src="https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white" alt="Flutter">
  <img src="https://img.shields.io/badge/Dart-0175C2?style=for-the-badge&logo=dart&logoColor=white" alt="Dart">
  <img src="https://img.shields.io/badge/GetX-800080?style=for-the-badge&logo=getx&logoColor=white" alt="GetX">
</div>

<hr>

<h2>🚀 Visão Geral</h2>
<p>
  O frontend do <strong>Presence+</strong> foca em uma experiência de usuário fluida para gestão de presenças. 
  A aplicação utiliza o <code>GetMaterialApp</code> para um gerenciamento de rotas centralizado e performático.
</p>

<h2>🗺️ Fluxo de Navegação</h2>
<ul>
  <li><strong>Login (SignInScreen):</strong> Rota inicial configurada em <code>initialRoute</code> para autenticação de usuários.</li>
  <li><strong>Cadastro (CadastroPage):</strong> Interface para registro de novos usuários através da rota <code>/cadastro</code>.</li>
  <li><strong>Perfil (UsuarioPage):</strong> Tela principal pós-login, centralizando as informações do usuário.</li>
  <li><strong>Configurações (ConfiguracaoPage):</strong> Acessada via <code>/configuracao</code> para ajustes personalizados.</li>
</ul>

<h2>🛠️ Destaques Técnicos</h2>
<table>
  <tr>
    <td><strong>Gerenciamento de Rotas</strong></td>
    <td>Implementado com <code>AppPages.pages</code> do GetX para escalabilidade.</td>
  </tr>
  <tr>
    <td><strong>Navegação</strong></td>
    <td>Uso de rotas nomeadas com <code>Navigator.pushNamed</code>.</td>
  </tr>
  <tr>
    <td><strong>UI Architecture</strong></td>
    <td>Widgets modulares e independentes (Stateless) para melhor manutenção.</td>
  </tr>
</table>

<h2>💻 Estrutura de Inicialização (main.dart)</h2>
<pre><code>
void main() {
  runApp(const MyWidget());
}

// Configuração central com GetMaterialApp
return GetMaterialApp(
  title: 'Presence+',
  initialRoute: PagesRoutes.signInRoute,
  getPages: AppPages.pages,
);
</code></pre>

<hr>

<div align="center">
  <p>Desenvolvido com ❤️ para gestão inteligente de presença
