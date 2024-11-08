<link rel="stylesheet" href="https://fonts.googleapis.com/icon?family=Material+Icons">
<script>
    import LearnQuest_logo from '$lib/LearnQuest_logo.png';
</script>


<section>
    <!-- Menu Button -->
    <!-- svelte-ignore a11y_click_events_have_key_events -->
     <i id="menu-btn" class="fas fa-bars"></i>
     
    <!-- Sidebar -->
    <div class="sidebar" id="sidebar">
        <img src={LearnQuest_logo} alt="LearnQuest Logo" class="logo"/>
        <a href="math.html">Math</a>
        <a href="science.html">English</a>
        <a href="ss.html">Science</a>
        <em><a href="makeyourown.html">Create Your Own</a></em>
    </div>

    <!-- Main content -->
    <div class="main" id="main-content">
        <!-- Header -->
        <div class="header">
            <h1>Welcome to LearnQuest</h1>
            <h3>LearnQuest: Ignite Curiosity, Achieve Excellence</h3>
            <p>Check our our latest review activities for our libraries, consisting of leassons from grades K-5.</p>
        </div>


        <div class="container math" id="home">
            <h3><pre class="material-icons" style="font-size:29px; color: #6a1b9a; vertical-align: middle; margin-right: 5px">calculate</pre>Math <span class="quest">Quests</span></h3>

            <div class="grade-list-container">
                <a href="math_kindergarten.html" class="link">
                    <span class="grade-item kindergarten">KG</span>
                </a>
                <a href="math_1st-grade.html" class="link">
                    <span class="grade-item first-grade">1st grade</span>
                </a>
                <a href="math_2nd-grade.html" class="link">
                    <span class="grade-item second-grade">2nd grade</span>
                </a>
                <a href="math_3rd-grade.html" class="link">
                    <span class="grade-item third-grade">3rd grade</span>
                </a>
                <a href="math_4th-grade.html" class="link">
                    <span class="grade-item fourth-grade">4th grade</span>
                </a>
                <a href="math_5th-grade.html" class="link">
                    <span class="grade-item fifth-grade">5th grade</span>
                </a>
            </div>
        </div>
        

        <div class="container english" id="services">
            <h3><pre class="material-icons" style="font-size:29px; color: #6a1b9a; vertical-align: middle; margin-right: 5px">menu_book</pre>English <span class="quest">Quests</span></h3>
        </div>

        <div class="container ss" id="home">
            <h3><pre class="material-icons" style="font-size:29px; color: #6a1b9a; vertical-align: middle; margin-right: 5px">history_edu</pre>Social Studies <span class="quest">Quests</span></h3>
        </div>

        <div class="container science" id="services">
            <h3><pre class="material-icons" style="font-size:29px; color: #6a1b9a; vertical-align: middle; margin-right: 5px">science</pre>Science <span class="quest">Quests</span></h3>
        </div>
    </div>

    <script>
        function openSidebar() {
            const sidebar = document.getElementById('sidebar');
            const mainContent = document.getElementById('main-content');
            if (sidebar.style.left === '0px') {
                sidebar.style.left = '-250px'; // Hide sidebar
                mainContent.style.marginLeft = '0'; // Reset main content margin
                document.getElementById("menu-btn").style.color = "#6a1b9a";
            } else {
                sidebar.style.left = '0px'; // Show sidebar
                mainContent.style.marginLeft = '250px'; // Adjust main content margin
                document.getElementById("menu-btn").style.color = "white";
            }
        }

        const button = document.getElementById('menu-btn');
        button.addEventListener('click', openSidebar);
    </script>
</section>
