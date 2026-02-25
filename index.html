<!DOCTYPE html>
<html lang="pt">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=yes">
    <title>BEAMOVE • sua rede fitness</title>
    
    <!-- Firebase SDK (compat para simplicidade) -->
    <script src="https://www.gstatic.com/firebasejs/10.7.1/firebase-app-compat.js"></script>
    <script src="https://www.gstatic.com/firebasejs/10.7.1/firebase-auth-compat.js"></script>
    <script src="https://www.gstatic.com/firebasejs/10.7.1/firebase-firestore-compat.js"></script>
    <script src="https://www.gstatic.com/firebasejs/10.7.1/firebase-storage-compat.js"></script>
    
    <!-- Cloudinary Upload Widget -->
    <script src="https://upload-widget.cloudinary.com/global/all.js"></script>
    
    <style>
        /* ===== RESET E PALETA OBRIGATÓRIA ===== */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;
        }

        :root {
            --offwhite: #F6F1EC;
            --marrom: #6B4C3B;
            --marrom-escuro: #3E2A22;
            --rose: #C49A8A;
        }

        body {
            background-color: var(--offwhite);
            color: var(--marrom-escuro);
            transition: background-color 0.3s, color 0.3s;
            min-height: 100vh;
        }

        /* Modo escuro */
        body.dark-mode {
            background-color: #1a1a1a;
            color: var(--offwhite);
        }
        body.dark-mode .card {
            background: #2C241F;
            color: var(--offwhite);
        }
        body.dark-mode .navbar {
            background: #2C241F;
            border-top-color: var(--marrom);
        }
        body.dark-mode input,
        body.dark-mode textarea,
        body.dark-mode select,
        body.dark-mode .settings-modal {
            background: #3a302b;
            color: var(--offwhite);
            border-color: var(--marrom);
        }
        body.dark-mode .settings-modal {
            background: #2C241F;
        }
        body.dark-mode .conversation-item:hover {
            background: #3a302b;
        }

        /* ===== COMPONENTES GLOBAIS ===== */
        .hidden {
            display: none !important;
        }

        .center {
            display: flex;
            justify-content: center;
            align-items: center;
        }

        .btn {
            cursor: pointer;
            border: none;
            padding: 12px 24px;
            border-radius: 40px;
            background: var(--rose);
            color: white;
            font-weight: 600;
            font-size: 1rem;
            transition: all 0.2s;
            box-shadow: 0 2px 8px rgba(107, 76, 59, 0.2);
            margin: 8px 0;
            width: 100%;
        }

        .btn-outline {
            background: transparent;
            border: 1px solid var(--rose);
            color: var(--marrom);
        }

        body.dark-mode .btn-outline {
            color: var(--rose);
        }

        .btn-small {
            padding: 8px 16px;
            font-size: 0.9rem;
            width: auto;
        }

        input, textarea, select {
            width: 100%;
            padding: 12px 16px;
            margin: 8px 0;
            border-radius: 30px;
            border: 1px solid var(--rose);
            background: white;
            font-size: 1rem;
            outline: none;
        }

        /* Logo */
        .logo {
            font-size: 2.5rem;
            font-weight: 300;
            letter-spacing: -0.02em;
        }
        .logo .bea {
            color: var(--marrom);
            font-weight: 400;
        }
        .logo .move {
            color: var(--rose);
            position: relative;
            display: inline-block;
        }
        .logo .move .o-circle {
            display: inline-block;
            border: 1.5px solid var(--rose);
            border-radius: 50%;
            width: 1.1em;
            height: 1.1em;
            text-align: center;
            line-height: 1;
            margin-left: 2px;
            transform: translateY(2px);
            font-size: 0.9em;
        }
        .tagline {
            font-size: 0.8rem;
            color: var(--marrom);
            letter-spacing: 0.05rem;
            margin-top: 0.2rem;
        }

        /* ===== SPLASH ===== */
        .splash {
            position: fixed;
            inset: 0;
            background: var(--offwhite);
            z-index: 2000;
            flex-direction: column;
            text-align: center;
            padding: 40px;
            animation: fadeIn 1.5s ease;
            transition: opacity 0.6s;
        }
        .splash.fade-out {
            opacity: 0;
            pointer-events: none;
        }
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        .splash-name {
            font-size: 1.8rem;
            color: var(--marrom);
            margin: 1rem 0;
            font-weight: 300;
        }

        /* ===== LOGIN ===== */
        .auth-container {
            max-width: 400px;
            margin: 0 auto;
            padding: 30px;
            text-align: center;
            display: flex;
            flex-direction: column;
            justify-content: center;
            min-height: 100vh;
        }

        /* ===== APP CONTAINER ===== */
        .app-container {
            max-width: 500px;
            margin: 0 auto;
            min-height: 100vh;
            padding-bottom: 80px;
            position: relative;
            display: block;
        }

        /* Cards Horizontais */
        .horizontal-scroll {
            display: flex;
            overflow-x: auto;
            gap: 16px;
            padding: 10px 0 20px;
            scrollbar-width: thin;
            -webkit-overflow-scrolling: touch;
        }
        .horizontal-scroll::-webkit-scrollbar {
            height: 4px;
        }
        .horizontal-scroll::-webkit-scrollbar-thumb {
            background: var(--rose);
            border-radius: 10px;
        }
        .info-card {
            min-width: 150px;
            background: white;
            border-radius: 20px;
            padding: 15px;
            box-shadow: 0 4px 12px rgba(107, 76, 59, 0.1);
            cursor: pointer;
            transition: transform 0.2s;
        }
        body.dark-mode .info-card {
            background: #2C241F;
        }
        .info-card:hover {
            transform: translateY(-2px);
        }
        .info-card h4 {
            color: var(--marrom);
            margin-bottom: 5px;
        }
        .info-card p {
            font-size: 0.85rem;
            opacity: 0.8;
        }
        .info-card .icon {
            font-size: 2rem;
            margin-bottom: 10px;
        }

        /* Seções */
        .section {
            padding: 20px 15px 80px;
            display: none;
        }
        .section.active {
            display: block;
        }

        /* Cards */
        .card {
            background: white;
            padding: 20px;
            border-radius: 24px;
            margin-bottom: 20px;
            box-shadow: 0 6px 18px rgba(107, 76, 59, 0.05);
            border: 1px solid rgba(196, 154, 138, 0.2);
        }

        /* Feed */
        .feed-img {
            width: 100%;
            border-radius: 16px;
            margin-bottom: 10px;
        }

        /* Post da Comunidade */
        .community-post {
            display: flex;
            gap: 12px;
            margin-bottom: 15px;
        }
        .post-avatar {
            width: 50px;
            height: 50px;
            border-radius: 50%;
            object-fit: cover;
        }
        .post-content {
            flex: 1;
        }
        .post-header {
            display: flex;
            align-items: center;
            gap: 8px;
            margin-bottom: 5px;
            flex-wrap: wrap;
        }
        .post-username {
            font-weight: 600;
            color: var(--marrom);
        }
        .post-category {
            font-size: 0.7rem;
            background: var(--rose);
            color: white;
            padding: 3px 8px;
            border-radius: 30px;
        }
        .post-text {
            margin: 10px 0;
            word-break: break-word;
        }
        .post-actions {
            display: flex;
            gap: 20px;
            margin-top: 10px;
            color: var(--marrom);
            flex-wrap: wrap;
        }
        .post-actions span {
            cursor: pointer;
            display: flex;
            align-items: center;
            gap: 5px;
            padding: 5px 10px;
            border-radius: 20px;
            transition: background 0.2s;
        }
        .post-actions span:hover {
            background: rgba(196, 154, 138, 0.1);
        }

        /* Perfil */
        .profile-header {
            display: flex;
            align-items: center;
            gap: 20px;
            margin-bottom: 20px;
        }
        .profile-img {
            width: 90px;
            height: 90px;
            border-radius: 50%;
            object-fit: cover;
            background: var(--rose);
            cursor: pointer;
            border: 2px solid var(--rose);
        }
        .profile-info {
            flex: 1;
        }
        .profile-username {
            color: var(--marrom);
            font-size: 0.9rem;
            margin: 5px 0;
        }
        .profile-bio {
            margin: 5px 0;
            font-size: 0.95rem;
            word-break: break-word;
        }
        .profile-link {
            color: var(--rose);
            text-decoration: none;
            font-size: 0.9rem;
            display: inline-block;
            margin-top: 5px;
            word-break: break-all;
        }
        .stats {
            display: flex;
            gap: 20px;
            margin: 15px 0;
        }
        .stat-item {
            text-align: center;
            flex: 1;
        }
        .stat-number {
            font-weight: bold;
            font-size: 1.2rem;
        }
        .stat-label {
            font-size: 0.8rem;
            color: var(--marrom);
        }

        /* Menu inferior */
        .navbar {
            position: fixed;
            bottom: 0;
            left: 0;
            right: 0;
            background: white;
            display: flex;
            justify-content: space-around;
            padding: 12px 0 8px;
            border-top: 1px solid rgba(196, 154, 138, 0.3);
            max-width: 500px;
            margin: 0 auto;
            z-index: 100;
        }
        .nav-item {
            font-size: 0.75rem;
            text-align: center;
            color: var(--marrom);
            cursor: pointer;
            opacity: 0.6;
            transition: 0.2s;
        }
        .nav-item.active {
            opacity: 1;
            color: var(--rose);
        }
        .nav-item i { 
            font-size: 1.8rem; 
            display: block;
            margin-bottom: 4px;
        }

        /* Modal de Configurações */
        .settings-modal {
            position: fixed;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            background: white;
            padding: 25px;
            border-radius: 30px;
            max-width: 90%;
            width: 400px;
            z-index: 1000;
            box-shadow: 0 10px 40px rgba(0,0,0,0.2);
        }
        .modal-overlay {
            position: fixed;
            inset: 0;
            background: rgba(0,0,0,0.5);
            z-index: 999;
        }

        /* Chat */
        .conversation-list {
            max-height: 70vh;
            overflow-y: auto;
        }
        .conversation-item {
            display: flex;
            align-items: center;
            gap: 15px;
            padding: 15px;
            border-radius: 20px;
            cursor: pointer;
            transition: background 0.2s;
            border-bottom: 1px solid rgba(196, 154, 138, 0.2);
        }
        .conversation-item:hover {
            background: rgba(196, 154, 138, 0.1);
        }
        .conversation-item img {
            width: 50px;
            height: 50px;
            border-radius: 50%;
            object-fit: cover;
        }
        .conversation-info {
            flex: 1;
        }
        .conversation-name {
            font-weight: 600;
            margin-bottom: 3px;
        }
        .conversation-last-message {
            font-size: 0.85rem;
            opacity: 0.7;
            white-space: nowrap;
            overflow: hidden;
            text-overflow: ellipsis;
            max-width: 200px;
        }
        .chat-container {
            display: flex;
            flex-direction: column;
            height: 70vh;
        }
        .chat-messages {
            flex: 1;
            overflow-y: auto;
            padding: 15px;
            display: flex;
            flex-direction: column;
            gap: 10px;
        }
        .message {
            display: flex;
            margin-bottom: 5px;
        }
        .message.sent {
            justify-content: flex-end;
        }
        .message.received {
            justify-content: flex-start;
        }
        .message-text {
            max-width: 70%;
            padding: 12px 18px;
            border-radius: 25px;
            background: var(--rose);
            color: white;
            word-break: break-word;
        }
        .message.received .message-text {
            background: rgba(196, 154, 138, 0.2);
            color: var(--marrom-escuro);
        }
        body.dark-mode .message.received .message-text {
            color: var(--offwhite);
            background: #3a302b;
        }
        .chat-input-area {
            display: flex;
            gap: 10px;
            padding: 10px;
            background: white;
            border-radius: 30px;
            margin-top: 10px;
        }
        body.dark-mode .chat-input-area {
            background: #2C241F;
        }
        .chat-input-area input {
            margin: 0;
            flex: 1;
        }
        .chat-input-area button {
            width: auto;
            margin: 0;
        }

        /* Engrenagem */
        .settings-icon {
            position: absolute;
            top: 20px;
            right: 15px;
            font-size: 1.8rem;
            color: var(--marrom);
            cursor: pointer;
            z-index: 10;
        }

        /* Loading */
        .loading {
            text-align: center;
            padding: 20px;
            color: var(--marrom);
        }

        /* Empty states */
        .empty-state {
            text-align: center;
            padding: 40px 20px;
            color: var(--marrom);
            opacity: 0.7;
        }
    </style>
</head>
<body>

<!-- SPLASH SCREEN -->
<div id="splash" class="splash center">
    <div>
        <div class="logo">
            <span class="bea">BEA</span><span class="move">MOVE<span class="o-circle">O</span></span>
        </div>
        <div class="tagline">“Sem extremismos. Resultados sustentáveis.”</div>
        <div style="margin-top: 40px;">
            <p class="splash-name">Olá, sou a Beatriz Antunes</p>
            <p style="margin-top: 20px; max-width: 300px; color: var(--marrom-escuro);">
                Personal Trainer & Fundadora do BEAMOVE<br>
                Especialista em transformação muito além do corpo.
            </p>
        </div>
    </div>
</div>

<!-- TELA DE LOGIN/REGISTRO -->
<div id="authSection" class="auth-container">
    <div class="logo" style="margin-bottom: 20px;">
        <span class="bea">BEA</span><span class="move">MOVE<span class="o-circle">O</span></span>
    </div>
    <div class="tagline" style="margin-bottom: 30px;">“Sem extremismos. Resultados sustentáveis.”</div>
    
    <input type="email" id="email" placeholder="Seu e-mail" value="teste@beamove.com">
    <input type="password" id="password" placeholder="Sua senha" value="123456">
    <div id="registerFields" class="hidden">
        <input type="text" id="registerUsername" placeholder="@username (ex: @maria)">
        <input type="text" id="registerName" placeholder="Nome de exibição">
    </div>
    
    <button class="btn" onclick="handleLogin()">Entrar</button>
    <button class="btn btn-outline" onclick="toggleRegisterForm()">Criar conta</button>
    <button class="btn btn-outline" onclick="handleResetPassword()" style="background: transparent;">Esqueci minha senha</button>
    
    <div id="loginError" style="color: #c00; margin-top: 10px;"></div>
</div>

<!-- APLICAÇÃO PRINCIPAL -->
<div id="app" class="app-container hidden">

    <!-- FEED / INÍCIO -->
    <div id="inicio" class="section active">
        <h2 style="margin-bottom: 20px;">Início</h2>
        
        <!-- Cards de Informação Horizontal -->
        <div class="horizontal-scroll" id="infoCards">
            <div class="info-card" onclick="openInfoPage('treinos')">
                <div class="icon">💪</div>
                <h4>Treinos</h4>
                <p>Dicas e exercícios para potencializar seus resultados</p>
            </div>
            <div class="info-card" onclick="openInfoPage('receitas')">
                <div class="icon">🥗</div>
                <h4>Receitas</h4>
                <p>Pratos saudáveis e saborosos para o dia a dia</p>
            </div>
            <div class="info-card" onclick="openInfoPage('dietas')">
                <div class="icon">📋</div>
                <h4>Dietas</h4>
                <p>Planos alimentares para diferentes objetivos</p>
            </div>
            <div class="info-card" onclick="openInfoPage('tipos-dieta')">
                <div class="icon">🔬</div>
                <h4>Tipos de Dieta</h4>
                <p>Low carb, cetogênica, jejum intermitente e mais</p>
            </div>
            <div class="info-card" onclick="openInfoPage('exercicios')">
                <div class="icon">🏋️</div>
                <h4>Exercícios</h4>
                <p>Explicações detalhadas de cada movimento</p>
            </div>
        </div>

        <h3 style="margin: 20px 0 10px;">Feed da Comunidade</h3>
        <div id="feed" class="loading">Carregando...</div>
    </div>

    <!-- EXPLORAR -->
    <div id="explorar" class="section">
        <h2 style="margin-bottom: 20px;">Explorar</h2>
        
        <!-- Plano Nutricional -->
        <div class="card">
            <h3 style="color: var(--marrom);">🥗 Acompanhamento Nutricional</h3>
            <p style="margin: 15px 0;">Plano individualizado com Beatriz Antunes</p>
            <button class="btn" onclick="window.open('https://pay.hotmart.com/beamove-nutri', '_blank')">Adquirir via Hotmart</button>
            <button class="btn btn-outline" onclick="window.open('https://kiwify.com.br/beamove-nutri', '_blank')">Adquirir via Kiwify</button>
        </div>

        <!-- Cursos -->
        <div class="card">
            <img src="https://images.unsplash.com/photo-1544367567-0f2fcb009e0b?w=400" class="feed-img" onerror="this.src='https://via.placeholder.com/400?text=Yoga'">
            <h4>Yoga para mulher moderna</h4>
            <p>Transformação sustentável • 8 semanas</p>
            <p style="color: var(--marrom);">⭐ 4.9 (234 avaliações)</p>
            <button class="btn" onclick="window.open('https://cursos.beamove.com/yoga', '_blank')">Comprar Agora</button>
        </div>

        <div class="card">
            <img src="https://images.unsplash.com/photo-1518310383802-640c2de311b2?w=400" class="feed-img" onerror="this.src='https://via.placeholder.com/400?text=Emagrecimento'">
            <h4>Emagrecimento sustentável</h4>
            <p>Método sem extremismos</p>
            <button class="btn" onclick="window.open('https://cursos.beamove.com/emagrecer', '_blank')">Comprar Agora</button>
        </div>
    </div>

    <!-- COMUNIDADE -->
    <div id="comunidade" class="section">
        <h2 style="margin-bottom: 20px;">Comunidade BEAMOVE</h2>
        <div class="card">
            <select id="postCategory">
                <option value="Motivação">🔥 Motivação</option>
                <option value="Dieta">🥗 Dieta</option>
                <option value="Receita">🍳 Receita</option>
                <option value="Treino">💪 Treino</option>
                <option value="Dúvida">❓ Dúvida</option>
            </select>
            <textarea id="communityText" placeholder="Compartilhe algo com a comunidade..." rows="3"></textarea>
            <button class="btn" onclick="postToCommunity()">Publicar</button>
        </div>
        <div id="communityPosts"></div>
    </div>

    <!-- CHAT -->
    <div id="chat" class="section">
        <div id="conversationsView">
            <h2 style="margin-bottom: 20px;">Conversas</h2>
            <div id="conversationsList" class="conversation-list">
                <div class="loading">Carregando conversas...</div>
            </div>
        </div>
        <div id="chatView" class="hidden">
            <button class="btn btn-small btn-outline" onclick="backToConversations()" style="margin-bottom: 10px;">← Voltar</button>
            <div id="currentChat" class="chat-container">
                <div id="chatMessages" class="chat-messages"></div>
                <div class="chat-input-area">
                    <input type="text" id="messageInput" placeholder="Digite sua mensagem..." onkeypress="if(event.key==='Enter') sendMessage()">
                    <button class="btn btn-small" onclick="sendMessage()">Enviar</button>
                </div>
            </div>
        </div>
    </div>

    <!-- PERFIL -->
    <div id="perfil" class="section">
        <div class="settings-icon" onclick="openSettings()">⚙️</div>
        
        <div class="profile-header">
            <img id="profileImage" class="profile-img" src="https://res.cloudinary.com/dgfm3rorv/image/upload/v1710101040/avatar.jpg" onclick="uploadProfileImage()">
            <div class="profile-info">
                <h3 id="profileDisplayName">Carregando...</h3>
                <p id="profileUsername" class="profile-username"></p>
                <p id="profileBio" class="profile-bio"></p>
                <a id="profileLink" class="profile-link" target="_blank"></a>
            </div>
        </div>

        <div class="stats">
            <div class="stat-item">
                <div class="stat-number" id="followersCount">0</div>
                <div class="stat-label">seguidores</div>
            </div>
            <div class="stat-item">
                <div class="stat-number" id="followingCount">0</div>
                <div class="stat-label">seguindo</div>
            </div>
        </div>

        <button class="btn btn-outline" onclick="showEditProfile()" style="margin: 15px 0;">Editar Perfil</button>

        <!-- Formulário do plano nutricional -->
        <div class="card">
            <h4>📋 Plano Nutricional Personalizado</h4>
            <p>Preencha para receber via WhatsApp</p>
            <input type="number" id="weight" placeholder="Peso (kg)">
            <input type="number" id="height" placeholder="Altura (cm)">
            <input type="text" id="goal" placeholder="Objetivo">
            <input type="text" id="restrictions" placeholder="Restrições alimentares">
            <textarea id="routine" placeholder="Rotina diária"></textarea>
            <button class="btn" onclick="sendToWhatsApp()">Enviar para consultoria</button>
        </div>
    </div>

    <!-- MENU INFERIOR -->
    <div class="navbar">
        <div class="nav-item active" onclick="showSection('inicio')">
            <i>🏠</i><span>Início</span>
        </div>
        <div class="nav-item" onclick="showSection('explorar')">
            <i>🔍</i><span>Explorar</span>
        </div>
        <div class="nav-item" onclick="showSection('comunidade')">
            <i>👥</i><span>Comunidade</span>
        </div>
        <div class="nav-item" onclick="showSection('chat')">
            <i>💬</i><span>Chat</span>
        </div>
        <div class="nav-item" onclick="showSection('perfil')">
            <i>👤</i><span>Perfil</span>
        </div>
    </div>
</div>

<!-- MODAL DE CONFIGURAÇÕES -->
<div id="settingsModal" class="hidden">
    <div class="modal-overlay" onclick="closeSettings()"></div>
    <div class="settings-modal">
        <h3 style="margin-bottom: 20px;">Configurações</h3>
        <div style="margin: 20px 0;">
            <label>Modo Noturno</label>
            <button class="btn btn-small" onclick="toggleDarkMode()" id="darkModeBtn">🌓 Ativar</button>
        </div>
        <button class="btn btn-outline" onclick="logout()">Sair da conta</button>
        <button class="btn btn-small" onclick="closeSettings()" style="margin-top: 10px;">Fechar</button>
    </div>
</div>

<!-- MODAL DE EDIÇÃO DE PERFIL -->
<div id="editProfileModal" class="hidden">
    <div class="modal-overlay" onclick="closeEditProfile()"></div>
    <div class="settings-modal">
        <h3 style="margin-bottom: 20px;">Editar Perfil</h3>
        <input type="text" id="editDisplayName" placeholder="Nome de exibição">
        <textarea id="editBio" placeholder="Bio (até 250 caracteres)" maxlength="250" rows="3"></textarea>
        <input type="url" id="editLink" placeholder="Link (opcional)">
        <button class="btn" onclick="saveProfile()">Salvar</button>
        <button class="btn btn-outline" onclick="closeEditProfile()">Cancelar</button>
    </div>
</div>

<script>
    // ========== CONFIGURAÇÕES FIREBASE ==========
    const firebaseConfig = {
        apiKey: "AIzaSyBdIH1kKv_e4f25nubgQ9ED8hyfl-3FmbM",
        authDomain: "beamove-pro.firebaseapp.com",
        projectId: "beamove-pro",
        storageBucket: "beamove-pro.firebasestorage.app",
        messagingSenderId: "816563837877",
        appId: "1:816563837877:web:7d812c57fecc0338f117fc"
    };

    // Inicializar Firebase
    firebase.initializeApp(firebaseConfig);
    const auth = firebase.auth();
    const db = firebase.firestore();
    
    // ========== VARIÁVEIS GLOBAIS ==========
    let currentUser = null;
    let cloudinaryWidget = null;
    let currentChatWith = null;
    let currentConversationId = null;
    let unsubscribeChat = null;

    // ========== SPLASH ==========
    setTimeout(() => {
        document.getElementById('splash').classList.add('fade-out');
        setTimeout(() => {
            document.getElementById('splash').style.display = 'none';
        }, 600);
    }, 3000);

    // ========== CONFIGURAÇÃO CLOUDINARY ==========
    if (window.cloudinary) {
        cloudinaryWidget = cloudinary.createUploadWidget(
            {
                cloudName: "dgfm3rorv",
                uploadPreset: "beamove_preset",
                sources: ['local', 'camera', 'url'],
                multiple: false,
                maxFiles: 1,
                clientAllowedFormats: ['images'],
                maxFileSize: 10000000,
                theme: 'minimal',
                language: 'pt'
            },
            (error, result) => {
                if (!error && result && result.event === "success") {
                    const imageUrl = result.info.secure_url;
                    
                    if (window.uploadingProfile) {
                        db.collection('users').doc(currentUser.uid).update({
                            photoURL: imageUrl
                        }).then(() => {
                            document.getElementById('profileImage').src = imageUrl;
                        });
                        window.uploadingProfile = false;
                    }
                }
            }
        );
    }

    window.uploadProfileImage = function() {
        if (!currentUser) return;
        window.uploadingProfile = true;
        if (cloudinaryWidget) cloudinaryWidget.open();
    };

    // ========== AUTENTICAÇÃO ==========
    window.toggleRegisterForm = function() {
        const registerFields = document.getElementById('registerFields');
        registerFields.classList.toggle('hidden');
    };

    window.handleLogin = function() {
        const email = document.getElementById('email').value;
        const password = document.getElementById('password').value;
        
        auth.signInWithEmailAndPassword(email, password)
            .catch(error => {
                document.getElementById('loginError').innerHTML = 'Erro: ' + error.message;
            });
    };

    window.handleRegister = async function() {
        const email = document.getElementById('email').value;
        const password = document.getElementById('password').value;
        const username = document.getElementById('registerUsername').value.trim();
        const displayName = document.getElementById('registerName').value.trim() || email.split('@')[0];
        
        if (!email || !password || !username) {
            document.getElementById('loginError').innerHTML = 'Preencha email, senha e username';
            return;
        }
        
        if (!username.startsWith('@')) {
            document.getElementById('loginError').innerHTML = 'Username deve começar com @';
            return;
        }
        
        try {
            // Verificar se username já existe
            const usernameDoc = await db.collection('usernames').doc(username.toLowerCase()).get();
            if (usernameDoc.exists) {
                document.getElementById('loginError').innerHTML = 'Este username já está em uso';
                return;
            }
            
            // Criar usuário
            const cred = await auth.createUserWithEmailAndPassword(email, password);
            
            // Salvar username
            await db.collection('usernames').doc(username.toLowerCase()).set({
                uid: cred.user.uid
            });
            
            // Criar perfil do usuário
            await db.collection('users').doc(cred.user.uid).set({
                email: email,
                username: username,
                displayName: displayName,
                bio: 'Movimento com propósito 🌱',
                link: '',
                photoURL: '',
                followers: 0,
                following: 0,
                createdAt: firebase.firestore.FieldValue.serverTimestamp()
            });
            
        } catch (error) {
            document.getElementById('loginError').innerHTML = 'Erro: ' + error.message;
        }
    };

    window.handleResetPassword = function() {
        const email = document.getElementById('email').value;
        if (!email) {
            alert('Digite seu e-mail primeiro');
            return;
        }
        auth.sendPasswordResetEmail(email)
            .then(() => alert('E-mail de recuperação enviado!'))
            .catch(error => alert('Erro: ' + error.message));
    };

    // Auth state observer
    auth.onAuthStateChanged(async user => {
        if (user) {
            currentUser = user;
            
            // Verificar se é registro ou login
            const userDoc = await db.collection('users').doc(user.uid).get();
            if (!userDoc.exists) {
                // Se não existe perfil, é um novo usuário que precisa completar registro
                return;
            }
            
            document.getElementById('authSection').classList.add('hidden');
            document.getElementById('app').classList.remove('hidden');
            
            loadFeed();
            loadProfile();
            loadCommunityPosts();
            loadConversations();
        } else {
            currentUser = null;
            document.getElementById('authSection').classList.remove('hidden');
            document.getElementById('app').classList.add('hidden');
            
            // Limpar campos
            document.getElementById('email').value = 'teste@beamove.com';
            document.getElementById('password').value = '123456';
            document.getElementById('registerFields').classList.add('hidden');
        }
    });

    // ========== NAVEGAÇÃO ==========
    window.showSection = function(sectionId) {
        document.querySelectorAll('.section').forEach(s => s.classList.remove('active'));
        document.getElementById(sectionId).classList.add('active');
        
        document.querySelectorAll('.nav-item').forEach((item, index) => {
            const sections = ['inicio', 'explorar', 'comunidade', 'chat', 'perfil'];
            item.classList.toggle('active', sections[index] === sectionId);
        });
        
        if (sectionId === 'inicio') loadFeed();
        if (sectionId === 'comunidade') loadCommunityPosts();
        if (sectionId === 'chat') {
            loadConversations();
            // Voltar para lista de conversas se estiver no chat
            backToConversations();
        }
        if (sectionId === 'perfil') loadProfile();
    };

    // ========== CARDS DE INFORMAÇÃO ==========
    window.openInfoPage = function(topic) {
        const content = {
            treinos: {
                title: '💪 Treinos Eficientes',
                text: 'Descubra treinos adaptados para sua rotina:\n\n• Treino de Força: 3x por semana\n• HIIT: 20 minutos, 2x por semana\n• Cardio: 30 minutos diários\n\nLembre-se: consistência é mais importante que intensidade!'
            },
            receitas: {
                title: '🥗 Receitas Saudáveis',
                text: 'Panqueca de Banana Fitness:\n• 1 banana amassada\n• 2 ovos\n• Canela a gosto\n• 1 colher de aveia\n\nModo: Bata tudo e asse em frigideira antiaderente.\n\nLow carb e delicioso!'
            },
            dietas: {
                title: '📋 Planos Alimentares',
                text: 'Uma dieta equilibrada deve conter:\n\n• Proteínas: frango, peixe, ovos\n• Carboidratos complexos: batata doce, arroz integral\n• Gorduras boas: abacate, azeite, castanhas\n• Fibras: vegetais, legumes'
            },
            'tipos-dieta': {
                title: '🔬 Tipos de Dieta',
                text: 'Low Carb: Redução de carboidratos (50-100g/dia)\nCetogênica: Alta em gorduras, muito baixo carboidrato\nJejum Intermitente: 16h jejum / 8h alimentação\nDieta Mediterrânea: Rica em azeite, peixes e vegetais'
            },
            exercicios: {
                title: '🏋️ Explicação de Exercícios',
                text: 'Agachamento: Pés na largura dos ombros, costas retas, desça como se fosse sentar numa cadeira.\n\nFlexão: Corpo reto, mãos na largura dos ombros, cotovelos a 45° do corpo.\n\nPrancha: Cotovelos no chão, corpo reto, contraia abdômen.'
            }
        };
        
        const data = content[topic];
        alert(`${data.title}\n\n${data.text}`);
    };

    // ========== FEED ==========
    function loadFeed() {
        const feed = document.getElementById('feed');
        feed.innerHTML = '<div class="loading">Carregando...</div>';
        
        db.collection('communityPosts').orderBy('createdAt', 'desc').limit(20).onSnapshot(snapshot => {
            if (snapshot.empty) {
                feed.innerHTML = '<div class="card empty-state">Nenhum post ainda. Seja o primeiro na comunidade!</div>';
                return;
            }
            
            let html = '';
            snapshot.forEach(doc => {
                const post = doc.data();
                const postId = doc.id;
                html += `
                    <div class="card">
                        <div class="community-post">
                            <img src="${post.photoURL || 'https://res.cloudinary.com/dgfm3rorv/image/upload/v1710101040/avatar.jpg'}" class="post-avatar" onclick="viewProfile('${post.userId}')">
                            <div class="post-content">
                                <div class="post-header">
                                    <span class="post-username" onclick="viewProfile('${post.userId}')">${post.username || post.displayName}</span>
                                    <span class="post-category">${post.category || 'Geral'}</span>
                                </div>
                                <div class="post-text">${post.text.replace(/\n/g, '<br>')}</div>
                                <div class="post-actions">
                                    <span onclick="likeCommunityPost('${postId}')">❤️ <span id="likes-${postId}">${post.likes || 0}</span></span>
                                    <span onclick="startChat('${post.userId}')">💬 Mensagem</span>
                                    ${post.userId !== currentUser?.uid ? `
                                        <span onclick="followUser('${post.userId}')" id="follow-${post.userId}">
                                            ${post.isFollowing ? '✓ Seguindo' : '➕ Seguir'}
                                        </span>
                                    ` : ''}
                                </div>
                            </div>
                        </div>
                    </div>
                `;
            });
            feed.innerHTML = html;
            
            // Verificar status de follow para cada post
            snapshot.forEach(doc => {
                const post = doc.data();
                if (post.userId !== currentUser?.uid) {
                    checkFollowStatus(post.userId);
                }
            });
        });
    }

    // ========== COMUNIDADE ==========
    window.postToCommunity = async function() {
        const text = document.getElementById('communityText').value;
        const category = document.getElementById('postCategory').value;
        
        if (!text.trim()) {
            alert('Digite algo para publicar');
            return;
        }
        
        try {
            const userDoc = await db.collection('users').doc(currentUser.uid).get();
            const userData = userDoc.data();
            
            await db.collection('communityPosts').add({
                userId: currentUser.uid,
                username: userData.username,
                displayName: userData.displayName,
                photoURL: userData.photoURL || '',
                text: text,
                category: category,
                likes: 0,
                createdAt: firebase.firestore.FieldValue.serverTimestamp()
            });
            
            document.getElementById('communityText').value = '';
            alert('Post publicado com sucesso!');
            
        } catch (error) {
            alert('Erro ao publicar: ' + error.message);
        }
    };

    function loadCommunityPosts() {
        const postsDiv = document.getElementById('communityPosts');
        postsDiv.innerHTML = '<div class="loading">Carregando...</div>';
        
        db.collection('communityPosts').orderBy('createdAt', 'desc').onSnapshot(snapshot => {
            if (snapshot.empty) {
                postsDiv.innerHTML = '<div class="card empty-state">Nenhuma postagem ainda. Seja o primeiro!</div>';
                return;
            }
            
            let html = '';
            snapshot.forEach(doc => {
                const post = doc.data();
                const postId = doc.id;
                html += `
                    <div class="card">
                        <div class="community-post">
                            <img src="${post.photoURL || 'https://res.cloudinary.com/dgfm3rorv/image/upload/v1710101040/avatar.jpg'}" class="post-avatar" onclick="viewProfile('${post.userId}')">
                            <div class="post-content">
                                <div class="post-header">
                                    <span class="post-username" onclick="viewProfile('${post.userId}')">${post.username || post.displayName}</span>
                                    <span class="post-category">${post.category || 'Geral'}</span>
                                </div>
                                <div class="post-text">${post.text.replace(/\n/g, '<br>')}</div>
                                <div class="post-actions">
                                    <span onclick="likeCommunityPost('${postId}')">❤️ <span id="community-likes-${postId}">${post.likes || 0}</span></span>
                                    <span onclick="startChat('${post.userId}')">💬 Mensagem</span>
                                    ${post.userId !== currentUser?.uid ? `
                                        <span onclick="followUser('${post.userId}')" id="community-follow-${post.userId}">
                                            ${post.isFollowing ? '✓ Seguindo' : '➕ Seguir'}
                                        </span>
                                    ` : ''}
                                </div>
                            </div>
                        </div>
                    </div>
                `;
            });
            postsDiv.innerHTML = html;
            
            // Verificar status de follow
            snapshot.forEach(doc => {
                const post = doc.data();
                if (post.userId !== currentUser?.uid) {
                    checkFollowStatus(post.userId);
                }
            });
        });
    }

    window.likeCommunityPost = async function(postId) {
        try {
            const postRef = db.collection('communityPosts').doc(postId);
            await postRef.update({
                likes: firebase.firestore.FieldValue.increment(1)
            });
            
            // Atualizar UI
            const likesSpan = document.getElementById(`community-likes-${postId}`) || document.getElementById(`likes-${postId}`);
            if (likesSpan) {
                const currentLikes = parseInt(likesSpan.innerText) || 0;
                likesSpan.innerText = currentLikes + 1;
            }
        } catch (error) {
            console.error('Erro ao curtir:', error);
        }
    };

    // ========== PERFIL ==========
    function loadProfile() {
        if (!currentUser) return;
        
        db.collection('users').doc(currentUser.uid).onSnapshot(doc => {
            if (doc.exists) {
                const data = doc.data();
                document.getElementById('profileDisplayName').innerText = data.displayName || data.username;
                document.getElementById('profileUsername').innerText = data.username || '';
                document.getElementById('profileBio').innerText = data.bio || '';
                const linkElement = document.getElementById('profileLink');
                if (data.link) {
                    linkElement.innerText = data.link;
                    linkElement.href = data.link.startsWith('http') ? data.link : 'https://' + data.link;
                    linkElement.classList.remove('hidden');
                } else {
                    linkElement.classList.add('hidden');
                }
                document.getElementById('followersCount').innerText = data.followers || 0;
                document.getElementById('followingCount').innerText = data.following || 0;
                
                if (data.photoURL) {
                    document.getElementById('profileImage').src = data.photoURL;
                }
            }
        });
    }

    window.showEditProfile = function() {
        db.collection('users').doc(currentUser.uid).get().then(doc => {
            const data = doc.data();
            document.getElementById('editDisplayName').value = data.displayName || '';
            document.getElementById('editBio').value = data.bio || '';
            document.getElementById('editLink').value = data.link || '';
            document.getElementById('editProfileModal').classList.remove('hidden');
        });
    };

    window.closeEditProfile = function() {
        document.getElementById('editProfileModal').classList.add('hidden');
    };

    window.saveProfile = function() {
        const displayName = document.getElementById('editDisplayName').value;
        const bio = document.getElementById('editBio').value;
        const link = document.getElementById('editLink').value;
        
        if (bio.length > 250) {
            alert('Bio deve ter no máximo 250 caracteres');
            return;
        }
        
        db.collection('users').doc(currentUser.uid).update({
            displayName: displayName,
            bio: bio,
            link: link
        }).then(() => {
            closeEditProfile();
            loadProfile();
        }).catch(error => {
            alert('Erro ao salvar: ' + error.message);
        });
    };

    window.viewProfile = function(userId) {
        if (userId === currentUser?.uid) {
            showSection('perfil');
        } else {
            // Implementar visualização de perfil de outro usuário
            alert('Visualizar perfil de outro usuário (em breve)');
        }
    };

    // ========== SEGUIR USUÁRIOS ==========
    async function checkFollowStatus(userId) {
        if (!currentUser) return;
        
        const followRef = db.collection('followers').doc(userId).collection('userFollowers').doc(currentUser.uid);
        const doc = await followRef.get();
        
        const followButton = document.getElementById(`follow-${userId}`) || document.getElementById(`community-follow-${userId}`);
        if (followButton) {
            followButton.innerHTML = doc.exists ? '✓ Seguindo' : '➕ Seguir';
        }
    }

    window.followUser = async function(userId) {
        if (userId === currentUser.uid) {
            alert('Você não pode seguir a si mesmo');
            return;
        }
        
        try {
            const followRef = db.collection('followers').doc(userId).collection('userFollowers').doc(currentUser.uid);
            const followingRef = db.collection('following').doc(currentUser.uid).collection('userFollowing').doc(userId);
            
            const followDoc = await followRef.get();
            
            if (followDoc.exists) {
                // Deixar de seguir
                await followRef.delete();
                await followingRef.delete();
                await db.collection('users').doc(userId).update({
                    followers: firebase.firestore.FieldValue.increment(-1)
                });
                await db.collection('users').doc(currentUser.uid).update({
                    following: firebase.firestore.FieldValue.increment(-1)
                });
            } else {
                // Seguir
                await followRef.set({ followedAt: firebase.firestore.FieldValue.serverTimestamp() });
                await followingRef.set({ followedAt: firebase.firestore.FieldValue.serverTimestamp() });
                await db.collection('users').doc(userId).update({
                    followers: firebase.firestore.FieldValue.increment(1)
                });
                await db.collection('users').doc(currentUser.uid).update({
                    following: firebase.firestore.FieldValue.increment(1)
                });
            }
            
            // Atualizar UI
            checkFollowStatus(userId);
            
        } catch (error) {
            console.error('Erro ao seguir:', error);
        }
    };

    // ========== CHAT ==========
    function loadConversations() {
        const listDiv = document.getElementById('conversationsList');
        
        if (!currentUser) return;
        
        db.collection('conversations')
            .where('participants', 'array-contains', currentUser.uid)
            .orderBy('updatedAt', 'desc')
            .onSnapshot(snapshot => {
                if (snapshot.empty) {
                    listDiv.innerHTML = '<div class="card empty-state">Nenhuma conversa ainda. Clique em "Mensagem" em um post para começar!</div>';
                    return;
                }
                
                let html = '';
                let loadedCount = 0;
                const totalConversations = snapshot.size;
                
                snapshot.forEach(doc => {
                    const conv = doc.data();
                    const convId = doc.id;
                    const otherUserId = conv.participants.find(id => id !== currentUser.uid);
                    
                    db.collection('users').doc(otherUserId).get().then(userDoc => {
                        if (userDoc.exists) {
                            const user = userDoc.data();
                            html += `
                                <div class="conversation-item" onclick="openChat('${convId}', '${otherUserId}')">
                                    <img src="${user.photoURL || 'https://res.cloudinary.com/dgfm3rorv/image/upload/v1710101040/avatar.jpg'}">
                                    <div class="conversation-info">
                                        <div class="conversation-name">${user.displayName || user.username}</div>
                                        <div class="conversation-last-message">${conv.lastMessage || 'Clique para iniciar conversa'}</div>
                                    </div>
                                </div>
                            `;
                        }
                        
                        loadedCount++;
                        if (loadedCount === totalConversations) {
                            listDiv.innerHTML = html;
                        }
                    });
                });
            });
    }

    window.startChat = async function(otherUserId) {
        if (!currentUser) return;
        
        const conversationId = [currentUser.uid, otherUserId].sort().join('_');
        const convRef = db.collection('conversations').doc(conversationId);
        const conv = await convRef.get();
        
        if (!conv.exists) {
            await convRef.set({
                participants: [currentUser.uid, otherUserId],
                createdAt: firebase.firestore.FieldValue.serverTimestamp(),
                updatedAt: firebase.firestore.FieldValue.serverTimestamp(),
                lastMessage: ''
            });
        }
        
        openChat(conversationId, otherUserId);
        showSection('chat');
    };

    window.openChat = function(conversationId, otherUserId) {
        currentChatWith = otherUserId;
        currentConversationId = conversationId;
        
        document.getElementById('conversationsView').classList.add('hidden');
        document.getElementById('chatView').classList.remove('hidden');
        
        const messagesDiv = document.getElementById('chatMessages');
        messagesDiv.innerHTML = '<div class="loading">Carregando mensagens...</div>';
        
        // Limpar listener anterior
        if (unsubscribeChat) {
            unsubscribeChat();
        }
        
        // Listener para mensagens
        unsubscribeChat = db.collection('conversations').doc(conversationId)
            .collection('messages')
            .orderBy('createdAt')
            .onSnapshot(snapshot => {
                if (snapshot.empty) {
                    messagesDiv.innerHTML = '<div class="empty-state">Nenhuma mensagem ainda. Envie a primeira!</div>';
                    return;
                }
                
                let html = '';
                snapshot.forEach(doc => {
                    const msg = doc.data();
                    const isSent = msg.senderId === currentUser.uid;
                    const time = msg.createdAt ? new Date(msg.createdAt.toDate()).toLocaleTimeString() : '';
                    
                    html += `
                        <div class="message ${isSent ? 'sent' : 'received'}">
                            <div class="message-text">
                                ${msg.text}
                                <div style="font-size: 0.7rem; opacity: 0.7; margin-top: 5px;">${time}</div>
                            </div>
                        </div>
                    `;
                });
                messagesDiv.innerHTML = html;
                messagesDiv.scrollTop = messagesDiv.scrollHeight;
            });
    };

    window.sendMessage = async function() {
        const text = document.getElementById('messageInput').value;
        if (!text.trim() || !currentChatWith || !currentConversationId) return;
        
        try {
            // Adicionar mensagem
            await db.collection('conversations').doc(currentConversationId)
                .collection('messages')
                .add({
                    text: text,
                    senderId: currentUser.uid,
                    createdAt: firebase.firestore.FieldValue.serverTimestamp()
                });
            
            // Atualizar conversa
            await db.collection('conversations').doc(currentConversationId).update({
                lastMessage: text,
                updatedAt: firebase.firestore.FieldValue.serverTimestamp()
            });
            
            document.getElementById('messageInput').value = '';
            
        } catch (error) {
            console.error('Erro ao enviar mensagem:', error);
            alert('Erro ao enviar mensagem: ' + error.message);
        }
    };

    window.backToConversations = function() {
        document.getElementById('conversationsView').classList.remove('hidden');
        document.getElementById('chatView').classList.add('hidden');
        
        if (unsubscribeChat) {
            unsubscribeChat();
            unsubscribeChat = null;
        }
        
        currentChatWith = null;
        currentConversationId = null;
        loadConversations();
    };

    // ========== WHATSAPP ==========
    window.sendToWhatsApp = function() {
        const weight = document.getElementById('weight').value;
        const height = document.getElementById('height').value;
        const goal = document.getElementById('goal').value;
        const restrictions = document.getElementById('restrictions').value;
        const routine = document.getElementById('routine').value;
        
        if (!weight || !height || !goal) {
            alert('Preencha pelo menos peso, altura e objetivo');
            return;
        }
        
        const message = `*Dados do Plano Nutricional*%0A%0A` +
            `Peso: ${weight} kg%0A` +
            `Altura: ${height} cm%0A` +
            `Objetivo: ${goal}%0A` +
            `Restrições: ${restrictions || 'Nenhuma'}%0A` +
            `Rotina: ${routine || 'Não informada'}`;
        
        window.open(`https://wa.me/5511999999999?text=${message}`, '_blank');
    };

    // ========== CONFIGURAÇÕES E MODO ESCURO ==========
    window.openSettings = function() {
        document.getElementById('settingsModal').classList.remove('hidden');
    };

    window.closeSettings = function() {
        document.getElementById('settingsModal').classList.add('hidden');
    };

    window.toggleDarkMode = function() {
        document.body.classList.toggle('dark-mode');
        const btn = document.getElementById('darkModeBtn');
        btn.innerText = document.body.classList.contains('dark-mode') ? '☀️ Desativar' : '🌓 Ativar';
    };

    window.logout = function() {
        auth.signOut();
        closeSettings();
    };

    console.log('🚀 BEAMOVE versão corrigida carregada com sucesso!');
</script>

</body>
</html>
