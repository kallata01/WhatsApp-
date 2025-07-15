# WhatsApp-
Página 

ñp PRADO" Nº 1789,<br>
        Edif. Ex - Hotel Plaza. PISO 2, Of. "207",<br>
        La Paz, Bolivia
    </div>
    <input type="text" id="username" placeholder="Usuario" required>
    <input type="password" id="password" placeholder="Contraseña" required>
    <button onclick="login()">Ingresar</button>
</div>

<div class="content-container hidden" id="content-box">
    <h2>Bienvenido</h2>
    <div class="info">
        <strong>Nombre:</strong> Dr. Zamorano<br>
        <strong>Dirección:</strong><br>
        Av. 16 de Julio "EL PRADO" Nº 1789,<br>
        Edif. Ex - Hotel Plaza. PISO 2, Of. "207",<br>
        La Paz, Bolivia
    </div>
    <div class="logout">
        <button onclick="logout()">Cerrar sesión</button>
    </div>
</div>

<script>
    function login() {
        const user = document.getElementById('username').value;
        const pass = document.getElementById('password').value;

        if (user === 'drzamorano' && pass === '1234') {
            document.getElementById('login-box').classList.add('hidden');
            document.getElementById('content-box').classList.remove('hidden');
        } else {
            alert('Usuario o contraseña incorrectos');
        }
    }

    function logout() {
        document.getElementById('login-box').classList.remove('hidden');
        document.getElementById('content-box').classList.add('hidden');
        document.getElementById('username').value = '';
        document.getElementById('password').value = '';
    }
</script>

</body>
</html>
