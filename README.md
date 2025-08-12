<header class="text-center mb-16 md:mb-24">
 <img src="images/logo.png" alt="VisioDen ロ고" class="h-12 mx-auto mb-3">
 <h1 class="text-4xl md:text-5xl font-extrabold tracking-tight">
  VisioDen
 </h1>
 <p class="mt-3 text-lg md:text-xl text-slate-600 max-w-2xl mx-auto">
  Where Vision Meets Mastery.
 </p>
</header><html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>VisioDen: Interactive Brand Page</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;700;800&display=swap" rel="stylesheet">
    <!-- Chosen Palette: Calm Harmony -->
    <!-- Application Structure Plan: The SPA is designed as a narrative journey to introduce the VisioDen brand. It starts with a strong hero section using the 'Clear Brand Statement' to establish the core identity. This is followed by an interactive 'Slogan Explorer' to showcase the short, memorable taglines in an engaging way. The page then breaks down the brand's foundation into three 'Core Principles' (Craftsmanship, Technology, Quality) for clarity. A dedicated section highlights the key differentiator—collaboration 'With Technicians'. The page concludes with the 'Concise Vision' statement, leaving a powerful final impression. This narrative structure was chosen over a simple list of options because it tells a cohesive story, making the brand's identity more compelling and easier for potential clients and partners to understand and connect with. -->
    <!-- Visualization & Content Choices: 
        Report Info: 'Clear Brand Statement' -> Goal: Inform/Establish Identity -> Viz/Method: Prominent text block in a hero section. -> Interaction: None. -> Justification: Sets the foundational tone immediately. -> Library/Method: HTML/Tailwind.
        Report Info: 'Short & Direct Slogans' -> Goal: Inform/Memorable -> Viz/Method: Interactive text display area with a button. -> Interaction: User clicks to cycle through slogans with a fade effect. -> Justification: More engaging and focused than a static list. -> Library/Method: Vanilla JS/Tailwind.
        Report Info: Core concepts (craftsmanship, technology, quality) -> Goal: Organize/Clarify -> Viz/Method: Three-column grid with Unicode icons and descriptive text. -> Interaction: Subtle hover effects. -> Justification: Visually breaks down the brand promise into digestible pillars. -> Library/Method: HTML/Tailwind.
        Report Info: 'Concise Vision' -> Goal: Inspire/Conclude -> Viz/Method: Bold, impactful text in a dedicated final section. -> Interaction: None. -> Justification: Provides a strong, memorable closing statement. -> Library/Method: HTML/Tailwind.
    -->
    <!-- CONFIRMATION: NO SVG graphics used. NO Mermaid JS used. -->
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f8fafc; /* slate-50 */
            color: #1e293b; /* slate-800 */
        }
        .fade-in {
            animation: fadeIn 0.5s ease-in-out;
        }
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }
        .brand-icon {
            font-size: 2.5rem;
            line-height: 1;
            color: #0891b2; /* cyan-600 */
        }
    </style>
</head>
<body class="antialiased">

    <div id="app" class="container mx-auto px-4 sm:px-6 lg:px-8 py-12 md:py-20">

        <header class="text-center mb-16 md:mb-24">
            <h1 class="text-4xl md:text-5xl font-extrabold tracking-tight">
                VisioDen
            </h1>
            <p class="mt-3 text-lg md:text-xl text-slate-600 max-w-2xl mx-auto">
                Where Vision Meets Mastery.
            </p>
        </header>

        <main>
            <section id="about" class="mb-16 md:mb-24 fade-in">
                <div class="bg-white p-8 md:p-12 rounded-2xl shadow-sm border border-slate-200 max-w-4xl mx-auto">
                    <h2 class="text-2xl md:text-3xl font-bold text-center mb-6">Redefining Dental Innovation</h2>
                    <p class="text-base md:text-lg text-slate-700 leading-relaxed text-center">
                        Founded by master dental technicians, VisioDen blends expert craftsmanship with advanced technology. We don't just make products <em>for</em> labs—we design them <em>with</em> labs, ensuring every detail delivers exceptional quality and performance.
                    </p>
                </div>
            </section>
            
            <section id="slogans" class="text-center mb-16 md:mb-24 fade-in" style="animation-delay: 0.2s;">
                 <div class="max-w-3xl mx-auto">
                    <h3 class="text-2xl font-bold mb-2">Our Brand Voice</h3>
                    <p class="text-slate-600 mb-8">Explore the core messages that define our commitment.</p>
                    <div class="bg-white p-8 rounded-2xl shadow-sm border border-slate-200 min-h-[100px] flex items-center justify-center">
                        <p id="slogan-display" class="text-2xl md:text-3xl font-semibold text-cyan-700 transition-opacity duration-300"></p>
                    </div>
                    <button id="slogan-button" class="mt-6 bg-cyan-600 hover:bg-cyan-700 text-white font-bold py-3 px-8 rounded-full transition-transform transform hover:scale-105 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-cyan-500">
                        Next Slogan
                    </button>
                </div>
            </section>

            <section id="principles" class="mb-16 md:mb-24 fade-in" style="animation-delay: 0.4s;">
                <div class="text-center mb-12">
                     <h3 class="text-2xl font-bold mb-2">Our Core Principles</h3>
                     <p class="text-slate-600">The foundation of every product we create.</p>
                </div>
                <div class="grid grid-cols-1 md:grid-cols-3 gap-8 max-w-6xl mx-auto">
                    <div class="bg-white p-8 rounded-2xl shadow-sm border border-slate-200 text-center hover:shadow-md transition-shadow duration-300">
                        <div class="brand-icon mb-4">👐</div>
                        <h4 class="text-xl font-bold mb-2">Expert Craftsmanship</h4>
                        <p class="text-slate-600">Born from the hands of master technicians who live and breathe the craft.</p>
                    </div>
                    <div class="bg-white p-8 rounded-2xl shadow-sm border border-slate-200 text-center hover:shadow-md transition-shadow duration-300">
                        <div class="brand-icon mb-4">🔬</div>
                        <h4 class="text-xl font-bold mb-2">Advanced Engineering</h4>
                        <p class="text-slate-600">Combining artistry with cutting-edge technology for precision production.</p>
                    </div>
                    <div class="bg-white p-8 rounded-2xl shadow-sm border border-slate-200 text-center hover:shadow-md transition-shadow duration-300">
                        <div class="brand-icon mb-4">✨</div>
                        <h4 class="text-xl font-bold mb-2">Uncompromising Quality</h4>
                        <p class="text-slate-600">Meticulously tested to meet the real-world demands of laboratory work.</p>
                    </div>
                </div>
            </section>
            
            <section id="vision" class="fade-in" style="animation-delay: 0.6s;">
                 <div class="bg-slate-800 text-white p-8 md:p-16 rounded-2xl text-center max-w-4xl mx-auto">
                    <h3 class="text-2xl md:text-4xl font-extrabold tracking-tight">
                        Dental innovation, redefined by experts.
                    </h3>
                    <p class="mt-4 text-base md:text-lg text-slate-300 max-w-2xl mx-auto">
                        We are master technicians creating the high-end solutions we've always wanted. This is where vision becomes reality.
                    </p>
                </div>
            </section>

        </main>

        <footer class="text-center mt-16 md:mt-24 pt-8 border-t border-slate-200">
            <p class="text-slate-500">&copy; 2025 VisioDen. All Rights Reserved.</p>
        </footer>

    </div>

    <script>
        document.addEventListener('DOMContentLoaded', function () {
            const slogans = [
                "By Technicians, For Technicians.",
                "The Technician's Choice.",
                "Where Vision Meets Mastery.",
                "Precision in Hand."
            ];
            let currentSloganIndex = 0;

            const sloganDisplay = document.getElementById('slogan-display');
            const sloganButton = document.getElementById('slogan-button');

            function updateSlogan() {
                sloganDisplay.classList.remove('fade-in');
                void sloganDisplay.offsetWidth; 
                sloganDisplay.classList.add('fade-in');
                sloganDisplay.textContent = slogans[currentSloganIndex];
            }

            sloganButton.addEventListener('click', () => {
                currentSloganIndex = (currentSloganIndex + 1) % slogans.length;
                updateSlogan();
            });

            updateSlogan();
        });
    </script>
</body>
</html>
