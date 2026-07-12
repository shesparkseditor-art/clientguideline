<!DOCTYPE html>
<html lang="id" class="light">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Personal Branding Agency - Video Guideline Pro</title>
    <!-- Tailwind CSS with Dark Mode Configuration -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Lucide Icons -->
    <script src="https://unpkg.com/lucide@latest"></script>
    
    <script>
        tailwind.config = {
            darkMode: 'class',
            theme: {
                extend: {
                    fontFamily: {
                        sans: [
                            '-apple-system', 
                            'BlinkMacSystemFont', 
                            '"SF Pro Display"', 
                            '"SF Pro Text"', 
                            '"SF Pro"', 
                            '"Segoe UI"', 
                            'Roboto', 
                            'sans-serif'
                        ],
                    },
                    colors: {
                        brand: {
                            50: '#f0f7ff',
                            100: '#e0f0fe',
                            200: '#bae2fd',
                            300: '#7cc9fc',
                            400: '#38adf8',
                            500: '#0e93eb',
                            600: '#0275c7',
                            700: '#035da1',
                            800: '#075085',
                            900: '#0c436e',
                        }
                    },
                    borderRadius: {
                        '4xl': '2rem',
                    }
                }
            }
        }
    </script>
    
    <style>
        body {
            font-family: -apple-system, BlinkMacSystemFont, "SF Pro Display", "SF Pro Text", "SF Pro", "Segoe UI", Roboto, sans-serif;
        }
        body.light-theme {
            background-color: #f1f8fe;
            background-image: 
                radial-gradient(at 0% 0%, hsla(202,81%,92%,1) 0px, transparent 50%),
                radial-gradient(at 100% 0%, hsla(186,84%,93%,1) 0px, transparent 50%),
                radial-gradient(at 100% 100%, hsla(204,100%,96%,1) 0px, transparent 50%),
                radial-gradient(at 0% 100%, hsla(201,84%,92%,1) 0px, transparent 50%);
            background-attachment: fixed;
        }

        body.dark-theme {
            background-color: #0b0f19;
            background-image: 
                radial-gradient(at 0% 0%, hsla(215, 40%, 12%, 1) 0px, transparent 50%),
                radial-gradient(at 100% 0%, hsla(220, 35%, 15%, 1) 0px, transparent 50%),
                radial-gradient(at 100% 100%, hsla(213, 45%, 11%, 1) 0px, transparent 50%),
                radial-gradient(at 0% 100%, hsla(217, 30%, 14%, 1) 0px, transparent 50%);
            background-attachment: fixed;
        }

        /* Custom Modern Scrollbars */
        ::-webkit-scrollbar {
            width: 6px;
            height: 6px;
        }
        ::-webkit-scrollbar-track {
            background: transparent;
        }
        ::-webkit-scrollbar-thumb {
            background: #bae2fd;
            border-radius: 9999px;
        }
        .dark-theme ::-webkit-scrollbar-thumb {
            background: #1e293b;
        }
        ::-webkit-scrollbar-thumb:hover {
            background: #7cc9fc;
        }
        
        .glass-card {
            background: rgba(255, 255, 255, 0.82);
            backdrop-filter: blur(20px);
            -webkit-backdrop-filter: blur(20px);
            border: 1px solid rgba(255, 255, 255, 0.7);
        }
        .dark .glass-card {
            background: rgba(15, 23, 42, 0.65);
            backdrop-filter: blur(20px);
            -webkit-backdrop-filter: blur(20px);
            border: 1px solid rgba(255, 255, 255, 0.06);
        }
        .slide-transition {
            transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
        }

        /* Orbit item layouts */
        .orbit-item {
            position: absolute;
            top: 50%;
            left: 50%;
            margin-top: -2.25rem; /* half of height */
            margin-left: -2.25rem; /* half of width */
            width: 4.5rem;
            height: 4.5rem;
        }
    </style>
</head>
<body class="min-h-screen font-sans text-slate-800 dark:text-slate-200 antialiased selection:bg-brand-200 light-theme overflow-x-hidden">

<script type="module">
    import { initializeApp } from "https://www.gstatic.com/firebasejs/11.6.1/firebase-app.js";
    import { getAuth, signInAnonymously, signInWithCustomToken, onAuthStateChanged } from "https://www.gstatic.com/firebasejs/11.6.1/firebase-auth.js";
    import { getFirestore, doc, setDoc, getDoc, updateDoc, collection, onSnapshot, addDoc, deleteDoc } from "https://www.gstatic.com/firebasejs/11.6.1/firebase-firestore.js";

    const appId = typeof __app_id !== 'undefined' ? __app_id : 'agency-guideline-manager-v5';
    const fallbackConfig = {
        apiKey: "mock-api-key-for-development-purposes",
        authDomain: "mock-auth-domain.firebaseapp.com",
        projectId: "mock-project-id",
        storageBucket: "mock-storage-bucket.appspot.com",
        messagingSenderId: "123456789",
        appId: "mock-app-id"
    };
    
    const firebaseConfig = typeof __firebase_config !== 'undefined' ? JSON.parse(__firebase_config) : fallbackConfig;
    
    let app, db, auth;
    let isFirebaseOnline = false;

    // Secure credentials configuration (Easier Passwords)
    const DEFAULT_USERS = [
        { id: 'director@agency', password: 'dir', role: 'Director', name: 'Director Utama', username: 'director@agency', avatar: '👑' },
        { id: 'senior@agency', password: 'snr', role: 'Senior Editor', name: 'Senior Editor', username: 'senior@agency', avatar: '⚡' },
        { id: 'dina@agency', password: 'dina', role: 'Dina', name: 'Dina', username: 'dina@agency', avatar: '✍️' },
        { id: 'nopi@agency', password: 'nopi', role: 'Nopi', name: 'Nopi', username: 'nopi@agency', avatar: '🎬' },
        { id: 'diva@agency', password: 'diva', role: 'Diva', name: 'Diva', username: 'diva@agency', avatar: '🎨' }
    ];

    let MOCK_USERS = JSON.parse(localStorage.getItem('agency_user_credentials_v2')) || DEFAULT_USERS;

    function saveUsersToLocalStorage() {
        localStorage.setItem('agency_user_credentials_v2', JSON.stringify(MOCK_USERS));
    }

    // STATE MANAGER
    let state = {
        welcomeSessionActive: true, 
        showLoginPanel: false, 
        currentUser: null,
        impersonatedRole: null,  
        clients: [],
        activeClientId: null,
        activeTab: 'short', // short, long, carousel
        sidebarActiveTab: 'dashboard', 
        searchQuery: '',
        isLoading: true,
        showNewClientModal: false,
        clientToDeleteId: null, 
        audioCtx: null,
        darkMode: false,
        sidebarCollapsed: false,
        mobileSidebarOpen: false, 
        activeSlideIndexes: {}, // key: client.id
        activeVideoIndexes: {}, // key: client.id-tab-category
        settingsActiveTab: 'profile',
        welcomeOrbitAngle: 0,
        autoplayPaused: {} // key: client.id
    };

    // Mengekspos state ke window global agar dapat diakses dari event handler inline HTML
    window.state = state;

    let welcomeIntervalId = null;
    let autoPlayIntervalId = null;

    // Local Multi-Tab Sync Fallback via BroadcastChannel
    let syncChannel;
    try {
        syncChannel = new BroadcastChannel('agency_realtime_sync_v6');
        syncChannel.onmessage = (event) => {
            if (event.data && event.data.type === 'UPDATE_CLIENTS') {
                state.clients = event.data.clients;
                if (state.activeClientId && !state.clients.some(c => c.id === state.activeClientId)) {
                    state.activeClientId = state.clients.length > 0 ? state.clients[0].id : null;
                }
                renderApp();
            }
        };
    } catch (e) {
        console.warn("BroadcastChannel not supported in this sandbox context.");
    }

    function broadcastClientsUpdate() {
        if (syncChannel && !isFirebaseOnline) {
            syncChannel.postMessage({
                type: 'UPDATE_CLIENTS',
                clients: state.clients
            });
        }
    }

    function startWelcomeOrbitAnimation() {
        if (welcomeIntervalId) clearInterval(welcomeIntervalId);
        welcomeIntervalId = setInterval(() => {
            if (state.welcomeSessionActive && !state.currentUser) {
                state.welcomeOrbitAngle -= 72; // Rotate
                
                const ringEl = document.getElementById('orbit-ring-rotator');
                if (ringEl) {
                    ringEl.style.transform = `rotate(${state.welcomeOrbitAngle}deg)`;
                    ringEl.style.transition = 'transform 1.1s cubic-bezier(0.25, 1, 0.5, 1)';
                    
                    const items = document.querySelectorAll('.orbit-inner-face');
                    items.forEach(el => {
                        el.style.transform = `rotate(${-state.welcomeOrbitAngle}deg)`;
                        el.style.transition = 'transform 1.1s cubic-bezier(0.25, 1, 0.5, 1)';
                    });
                }
            }
        }, 3000); 
    }

    // Autoplay logic for Global Guideline Slides
    function startGlobalAutoplayLoop() {
        if (autoPlayIntervalId) clearInterval(autoPlayIntervalId);
        autoPlayIntervalId = setInterval(() => {
            if (state.currentUser && state.sidebarActiveTab === 'dashboard' && state.activeClientId) {
                const client = state.clients.find(c => c.id === state.activeClientId);
                if (client && client.guidelineSlides && client.guidelineSlides.length > 1) {
                    const clientId = client.id;
                    if (!state.autoplayPaused[clientId]) {
                        if (state.activeSlideIndexes[clientId] === undefined) {
                            state.activeSlideIndexes[clientId] = 0;
                        }
                        state.activeSlideIndexes[clientId] = (state.activeSlideIndexes[clientId] + 1) % client.guidelineSlides.length;
                        renderApp();
                    }
                }
            }
        }, 4000); // Transitions slide every 4 seconds
    }

    window.showToast = function(message, type = 'success') {
        const toast = document.getElementById('toast');
        const toastText = document.getElementById('toast-text');
        const toastIcon = document.getElementById('toast-icon');
        
        toastText.innerText = message;
        if (type === 'success') {
            toast.className = "fixed top-6 right-6 z-50 flex items-center gap-3 bg-emerald-50 border border-emerald-200 text-emerald-800 dark:bg-emerald-950 dark:border-emerald-900 dark:text-emerald-200 px-5 py-3.5 rounded-2xl shadow-xl transition-all duration-300 transform translate-y-0";
            toastIcon.innerHTML = `<i data-lucide="check-circle" class="w-5 h-5 text-emerald-500"></i>`;
        } else {
            toast.className = "fixed top-6 right-6 z-50 flex items-center gap-3 bg-rose-50 border border-rose-200 text-rose-800 dark:bg-rose-950 dark:border-rose-900 dark:text-rose-200 px-5 py-3.5 rounded-2xl shadow-xl transition-all duration-300 transform translate-y-0";
            toastIcon.innerHTML = `<i data-lucide="alert-circle" class="w-5 h-5 text-rose-500"></i>`;
        }
        lucide.createIcons();
        
        setTimeout(() => {
            toast.className = "fixed top-6 right-6 z-50 flex items-center gap-3 bg-white px-5 py-3.5 rounded-2xl shadow-xl transition-all duration-300 transform -translate-y-20 opacity-0 pointer-events-none";
        }, 4000);
    };

    window.forceDownload = function(url, filename) {
        if (!url || url === '#' || url === '') {
            const mockContent = "Mock Data: File binary untuk " + filename;
            const blob = new Blob([mockContent], { type: "application/octet-stream" });
            const mockUrl = URL.createObjectURL(blob);
            const anchor = document.createElement('a');
            anchor.href = mockUrl;
            anchor.download = filename;
            document.body.appendChild(anchor);
            anchor.click();
            document.body.removeChild(anchor);
            URL.revokeObjectURL(mockUrl);
            window.showToast(`Berhasil mengunduh ${filename}!`, 'success');
            return;
        }

        if (url.startsWith('data:')) {
            const anchor = document.createElement('a');
            anchor.href = url;
            anchor.download = filename;
            document.body.appendChild(anchor);
            anchor.click();
            document.body.removeChild(anchor);
            window.showToast(`Berhasil mengunduh ${filename}!`, 'success');
            return;
        }

        fetch(url)
            .then(res => {
                if (!res.ok) throw new Error('Gagal mengambil data file');
                return res.blob();
            })
            .then(blob => {
                const blobUrl = URL.createObjectURL(blob);
                const anchor = document.createElement('a');
                anchor.href = blobUrl;
                anchor.download = filename;
                document.body.appendChild(anchor);
                anchor.click();
                document.body.removeChild(anchor);
                URL.revokeObjectURL(blobUrl);
                window.showToast(`Berhasil mengunduh ${filename}!`, 'success');
            })
            .catch(err => {
                const anchor = document.createElement('a');
                anchor.href = url;
                anchor.download = filename;
                anchor.click();
            });
    };

    window.copyColorToClipboard = function(hexValue) {
        const tempTextArea = document.createElement("textarea");
        tempTextArea.value = hexValue;
        document.body.appendChild(tempTextArea);
        tempTextArea.select();
        try {
            document.execCommand('copy');
            window.showToast(`Warna ${hexValue} disalin ke clipboard!`, 'success');
        } catch (err) {
            window.showToast("Gagal menyalin warna.", "error");
        }
        document.body.removeChild(tempTextArea);
    };

    window.playSynthesizedSFX = function(type) {
        try {
            if (!state.audioCtx) {
                state.audioCtx = new (window.AudioContext || window.webkitAudioContext)();
            }
            const ctx = state.audioCtx;
            if (ctx.state === 'suspended') {
                ctx.resume();
            }
            const osc = ctx.createOscillator();
            const gain = ctx.createGain();
            osc.connect(gain);
            gain.connect(ctx.destination);

            if (type === 'clean-pop') {
                osc.type = 'sine';
                osc.frequency.setValueAtTime(380, ctx.currentTime);
                osc.frequency.exponentialRampToValueAtTime(1450, ctx.currentTime + 0.08);
                gain.gain.setValueAtTime(0.3, ctx.currentTime);
                gain.gain.exponentialRampToValueAtTime(0.01, ctx.currentTime + 0.1);
                osc.start(ctx.currentTime);
                osc.stop(ctx.currentTime + 0.1);
            } else if (type === 'whoosh') {
                osc.type = 'sine';
                osc.frequency.setValueAtTime(150, ctx.currentTime);
                osc.frequency.exponentialRampToValueAtTime(1400, ctx.currentTime + 0.35);
                gain.gain.setValueAtTime(0.01, ctx.currentTime);
                gain.gain.linearRampToValueAtTime(0.2, ctx.currentTime + 0.08);
                gain.gain.exponentialRampToValueAtTime(0.01, ctx.currentTime + 0.35);
                osc.start(ctx.currentTime);
                osc.stop(ctx.currentTime + 0.4);
            } else if (type === 'ding') {
                osc.type = 'triangle';
                osc.frequency.setValueAtTime(1046.50, ctx.currentTime);
                osc.frequency.exponentialRampToValueAtTime(1567.98, ctx.currentTime + 0.15);
                gain.gain.setValueAtTime(0.25, ctx.currentTime);
                gain.gain.exponentialRampToValueAtTime(0.01, ctx.currentTime + 0.5);
                osc.start(ctx.currentTime);
                osc.stop(ctx.currentTime + 0.5);
            } else if (type === 'pop') {
                osc.type = 'sine';
                osc.frequency.setValueAtTime(350, ctx.currentTime);
                osc.frequency.quadraticRampToValueAtTime(90, ctx.currentTime + 0.1);
                gain.gain.setValueAtTime(0.4, ctx.currentTime);
                gain.gain.exponentialRampToValueAtTime(0.01, ctx.currentTime + 0.12);
                osc.start(ctx.currentTime);
                osc.stop(ctx.currentTime + 0.12);
            } else if (type === 'swoosh') {
                osc.type = 'sawtooth';
                osc.frequency.setValueAtTime(90, ctx.currentTime);
                osc.frequency.exponentialRampToValueAtTime(700, ctx.currentTime + 0.25);
                gain.gain.setValueAtTime(0.15, ctx.currentTime);
                gain.gain.exponentialRampToValueAtTime(0.01, ctx.currentTime + 0.3);
                osc.start(ctx.currentTime);
                osc.stop(ctx.currentTime + 0.3);
            }
        } catch (err) {
            console.log("Audio synthesis active with restrictions");
        }
    };

    let dragStartX = 0;
    let dragIsActive = false;

    window.handleSlideTouchStart = function(e) {
        dragStartX = e.touches[0].clientX;
        dragIsActive = true;
    };

    window.handleSlideTouchEnd = function(e, clientId, maxSlides) {
        if (!dragIsActive || maxSlides <= 1) return;
        const endX = e.changedTouches[0].clientX;
        const diffX = dragStartX - endX;
        if (Math.abs(diffX) > 40) { 
            state.autoplayPaused[clientId] = true; // Pause auto-loop on manual interaction
            if (diffX > 0) {
                window.changeSlideIndex(clientId, 1, maxSlides);
            } else {
                window.changeSlideIndex(clientId, -1, maxSlides);
            }
        }
        dragIsActive = false;
    };

    window.handleSlideMouseDown = function(e) {
        dragStartX = e.clientX;
        dragIsActive = true;
    };

    window.handleSlideMouseUp = function(e, clientId, maxSlides) {
        if (!dragIsActive || maxSlides <= 1) return;
        const endX = e.clientX;
        const diffX = dragStartX - endX;
        if (Math.abs(diffX) > 40) { 
            state.autoplayPaused[clientId] = true; // Pause auto-loop on manual interaction
            if (diffX > 0) {
                window.changeSlideIndex(clientId, 1, maxSlides);
            } else {
                window.changeSlideIndex(clientId, -1, maxSlides);
            }
        }
        dragIsActive = false;
    };

    const createEmptyTab = (formatName) => {
        const data = {
            description: '',
            links: [
                { id: 'link-init-1', title: 'Referensi Gaya Instagram', url: 'https://www.instagram.com/reel/C8vUxyfpe11/' }
            ],
            contohOutput: []
        };

        if (formatName === 'long') {
            data.contohOutput = [
                { id: 'co-init-1', name: 'Contoh B-Roll Premium', url: 'https://assets.mixkit.co/videos/preview/mixkit-man-holding-a-smartphone-in-his-hand-40545-large.mp4', note: 'Potong b-roll setiap 2.5 detik sekali untuk menjaga tempo.', subCategory: 'B-roll' },
                { id: 'co-init-2', name: 'Contoh Typography Pop', url: 'https://assets.mixkit.co/videos/preview/mixkit-hands-of-a-video-editor-using-a-computer-and-a-keyboard-40546-large.mp4', note: 'Teks utama wajib kuning neon, teks pembantu putih bersih.', subCategory: 'Typography' },
                { id: 'co-init-3', name: 'Contoh Animasi Hook', url: 'https://assets.mixkit.co/videos/preview/mixkit-set-of-keys-on-a-piano-keyboard-41586-large.mp4', note: 'Gunakan animasi pop bounce untuk sticker indikator.', subCategory: 'Animasi' }
            ];
            data.transitions = [
                { id: 'tr-init-1', title: 'Smooth Zoom Transition', description: 'Transisi zoom in dengan blur radial 10px', name: 'Zoom_Transition.jpg', url: 'https://images.unsplash.com/photo-1618005182384-a83a8bd57fbe?auto=format&fit=crop&w=400&q=80' }
            ];
            data.sfx = [
                { id: 'sfx-init-1', name: 'Whoosh Transition Fast', type: 'whoosh', url: '#' }
            ];
        } else if (formatName === 'short') {
            data.contohOutput = [
                { id: 'co-short-1', title: 'Contoh Hook Short Portrait', url: 'https://assets.mixkit.co/videos/preview/mixkit-man-holding-a-smartphone-in-his-hand-40545-large.mp4', description: 'Gunakan pancingan visual (Hook) di 3 detik awal.' }
            ];
        } else if (formatName === 'carousel') {
            data.contohOutput = [
                { id: 'co-carousel-1', title: 'Slide Cover 4:5 Minimalis', url: 'https://images.unsplash.com/photo-1611162617213-7d7a39e9b1d7?auto=format&fit=crop&w=800&q=80', description: 'Gunakan font Serif elegan dengan ukuran kontras tinggi.' }
            ];
        }

        return data;
    };

    // Global Guideline Slides direct parent attributes
    const INITIAL_CLIENTS = [
        {
            id: 'client-1',
            name: 'Raffi Ahmad Personal Brand',
            logo: 'https://images.unsplash.com/photo-1534528741775-53994a69daeb?auto=format&fit=crop&w=256&q=80',
            assignedEditor: 'Dina',
            colorPalette: [
                { id: 'col-init-1', hex: '#FF3E6C', name: 'Accent Rose' },
                { id: 'col-init-2', hex: '#00E5FF', name: 'Neon Sky' },
                { id: 'col-init-3', hex: '#1C2035', name: 'Dark Navy' }
            ],
            graphicElements: [
                { id: 'ge-init-1', title: 'Stiker Sparkle Neon', description: 'Gunakan di setiap transisi utama atau overlay penekanan kata.', name: 'Sparkles Element.png', url: 'https://images.unsplash.com/photo-1599508704512-2f19efd1e35f?auto=format&fit=crop&w=400&q=80' }
            ],
            fonts: [
                { id: 'font-init-1', name: 'Montserrat Bold.zip', url: '#' }
            ],
            guidelineSlides: [
                { id: 'slide-init-1', imageUrl: 'https://images.unsplash.com/photo-1611162617213-7d7a39e9b1d7?auto=format&fit=crop&w=800&q=80', text: 'Slide 1: Pasang logo brand di tengah atas selama 1.5 detik pertama.' },
                { id: 'slide-init-2', imageUrl: 'https://images.unsplash.com/photo-1542744094-3a31f103e35f?auto=format&fit=crop&w=800&q=80', text: 'Slide 2: Tambahkan tulisan hook tebal dengan animasi slide up.' }
            ],
            short: createEmptyTab('short'),
            long: createEmptyTab('long'),
            carousel: createEmptyTab('carousel')
        },
        {
            id: 'client-2',
            name: 'Merry Riana Motivasi Brand',
            logo: 'https://images.unsplash.com/photo-1573496359142-b8d87734a5a2?auto=format&fit=crop&w=256&q=80',
            assignedEditor: 'Nopi',
            colorPalette: [
                { id: 'col-init-1', hex: '#E11D48', name: 'Merry Red' },
                { id: 'col-init-2', hex: '#FBBF24', name: 'Gold Accent' }
            ],
            graphicElements: [],
            fonts: [],
            guidelineSlides: [
                { id: 'slide-init-3', imageUrl: 'https://images.unsplash.com/photo-1551836022-d5d88e9218df?auto=format&fit=crop&w=800&q=80', text: 'Slide Utama: Komposisi pembicara berada tepat di garis tengah layar.' }
            ],
            short: createEmptyTab('short'),
            long: createEmptyTab('long'),
            carousel: createEmptyTab('carousel')
        },
        {
            id: 'client-3',
            name: 'Coach Rene Leadership',
            logo: 'https://images.unsplash.com/photo-1472099645785-5658abf4ff4e?auto=format&fit=crop&w=256&q=80',
            assignedEditor: 'Diva',
            colorPalette: [
                { id: 'col-init-1', hex: '#0284C7', name: 'Professional Blue' },
                { id: 'col-init-2', hex: '#0F172A', name: 'Ink Dark' }
            ],
            graphicElements: [],
            fonts: [],
            guidelineSlides: [
                { id: 'slide-init-4', imageUrl: 'https://images.unsplash.com/photo-1517245386807-bb43f82c33c4?auto=format&fit=crop&w=800&q=80', text: 'Slide Utama: Gunakan warna professional blue untuk teks sorotan.' }
            ],
            short: createEmptyTab('short'),
            long: createEmptyTab('long'),
            carousel: createEmptyTab('carousel')
        }
    ];

    window.toggleDarkMode = function(value) {
        state.darkMode = value;
        const html = document.documentElement;
        const body = document.body;
        if (state.darkMode) {
            html.classList.add('dark');
            body.classList.add('dark-theme');
            body.classList.remove('light-theme');
        } else {
            html.classList.remove('dark');
            body.classList.add('light-theme');
            body.classList.remove('dark-theme');
        }
        localStorage.setItem('agency_dark_mode', state.darkMode);
        renderApp();
    };

    window.toggleSidebar = function() {
        state.sidebarCollapsed = !state.sidebarCollapsed;
        renderApp();
    };

    window.toggleMobileSidebar = function() {
        state.mobileSidebarOpen = !state.mobileSidebarOpen;
        renderApp();
    };

    async function startAppAuthAndSync() {
        const savedDarkMode = localStorage.getItem('agency_dark_mode');
        if (savedDarkMode !== null) {
            window.toggleDarkMode(savedDarkMode === 'true');
        } else {
            window.toggleDarkMode(false);
        }

        startWelcomeOrbitAnimation();
        startGlobalAutoplayLoop();

        // Check if platform has supplied custom Firebase credentials
        if (typeof __firebase_config !== 'undefined') {
            try {
                const config = JSON.parse(__firebase_config);
                app = initializeApp(config);
                auth = getAuth(app);
                db = getFirestore(app);
                isFirebaseOnline = true;
            } catch (err) {
                console.warn("Could not bind custom Firebase. Utilizing fallback config.");
            }
        }

        // Falling back to standard config if needed
        if (!isFirebaseOnline) {
            try {
                app = initializeApp(fallbackConfig);
                auth = getAuth(app);
                db = getFirestore(app);
                isFirebaseOnline = true;
            } catch (err) {
                isFirebaseOnline = false;
            }
        }

        if (isFirebaseOnline && auth && db) {
            try {
                let userCredential;
                if (typeof __initial_auth_token !== 'undefined' && __initial_auth_token) {
                    userCredential = await signInWithCustomToken(auth, __initial_auth_token);
                } else {
                    userCredential = await signInAnonymously(auth);
                }
                
                const firebaseUser = userCredential.user;
                
                // Seed data to Firestore if completely empty
                const seedDocRef = doc(db, 'artifacts', appId, 'public', 'data', 'metadata', 'seeded');
                const seedSnap = await getDoc(seedDocRef);
                
                if (!seedSnap.exists()) {
                    for (const client of INITIAL_CLIENTS) {
                        const clientDocRef = doc(db, 'artifacts', appId, 'public', 'data', 'clients', client.id);
                        await setDoc(clientDocRef, client);
                    }
                    await setDoc(seedDocRef, { seededAt: new Date().toISOString() });
                }

                // Attach active snapshot listeners for real-time cloud data push
                const clientsCollection = collection(db, 'artifacts', appId, 'public', 'data', 'clients');
                onSnapshot(clientsCollection, (snapshot) => {
                    const loadedClients = [];
                    snapshot.forEach((doc) => {
                        loadedClients.push({ id: doc.id, ...doc.data() });
                    });
                    state.clients = loadedClients;
                    state.isLoading = false;
                    renderApp();
                }, (error) => {
                    loadLocalFallback();
                });
            } catch (err) {
                loadLocalFallback();
            }
        } else {
            loadLocalFallback();
        }
    }

    function loadLocalFallback() {
        state.clients = JSON.parse(localStorage.getItem('agency_clients_backup_v6')) || INITIAL_CLIENTS;
        state.isLoading = false;
        renderApp();
    }

    // Helper to sanitize files if memory is exceeded
    function stripLargeBase64(clients) {
        if (!clients) return [];
        try {
            return clients.map(client => {
                const copy = JSON.parse(JSON.stringify(client));
                if (copy.graphicElements) {
                    copy.graphicElements.forEach(item => {
                        if (item.url && item.url.startsWith('data:') && item.url.length > 50000) {
                            item.url = 'https://placehold.co/150x150/bae2fd/0e93eb?text=Graphic+Element';
                        }
                    });
                }
                if (copy.guidelineSlides) {
                    copy.guidelineSlides.forEach(slide => {
                        if (slide.imageUrl && slide.imageUrl.startsWith('data:') && slide.imageUrl.length > 50000) {
                            slide.imageUrl = 'https://images.unsplash.com/photo-1611162617213-7d7a39e9b1d7?auto=format&fit=crop&w=800&q=80';
                        }
                    });
                }
                const formats = ['short', 'long', 'carousel'];
                formats.forEach(format => {
                    if (copy[format]) {
                        if (copy[format].contohOutput) {
                            copy[format].contohOutput.forEach(v => {
                                if (v.url && v.url.startsWith('data:') && v.url.length > 50000) {
                                    v.url = ''; 
                                }
                            });
                        }
                    }
                });
                return copy;
            });
        } catch (e) {
            return clients;
        }
    }

    function saveLocalBackupIfOffline() {
        if (!isFirebaseOnline) {
            try {
                localStorage.setItem('agency_clients_backup_v6', JSON.stringify(state.clients));
            } catch (err) {
                try {
                    const sanitized = stripLargeBase64(state.clients);
                    localStorage.setItem('agency_clients_backup_v6', JSON.stringify(sanitized));
                } catch (innerErr) {
                    console.error("Quota warning - offline save adjusted.");
                }
            }
        }
        broadcastClientsUpdate();
    }

    window.onload = function() {
        startAppAuthAndSync();
    };

    window.updateClientName = async function(clientId, newName) {
        const trimmed = newName.trim();
        if (!trimmed) {
            window.showToast("Nama klien tidak boleh kosong!", "error");
            return;
        }
        const client = state.clients.find(c => c.id === clientId);
        if (client) {
            client.name = trimmed;
            await window.updateClientState(client);
            window.showToast("Nama klien berhasil diperbarui!", "success");
        }
    };

    window.confirmDeleteClient = function(clientId) {
        state.clientToDeleteId = clientId;
        renderApp();
    };

    window.cancelDeleteClient = function() {
        state.clientToDeleteId = null;
        renderApp();
    };

    window.executeDeleteClient = async function() {
        const id = state.clientToDeleteId;
        if (!id) return;

        if (isFirebaseOnline && db) {
            try {
                await deleteDoc(doc(db, 'artifacts', appId, 'public', 'data', 'clients', id));
            } catch (err) {
                console.error("Firebase delete failed, falling back to local only.");
            }
        }

        state.clients = state.clients.filter(c => c.id !== id);
        saveLocalBackupIfOffline();

        if (state.activeClientId === id) {
            state.activeClientId = state.clients.length > 0 ? state.clients[0].id : null;
        }

        state.clientToDeleteId = null;
        window.showToast("Klien berhasil dihapus secara permanen!", "success");
        renderApp();
    };

    window.togglePasswordVisibilityDirectly = function() {
        const pwdInput = document.getElementById('login-password-field');
        const eyeIcon = document.getElementById('password-eye-icon-holder');
        if (pwdInput) {
            if (pwdInput.type === 'password') {
                pwdInput.type = 'text';
                if (eyeIcon) eyeIcon.innerHTML = `<i data-lucide="eye-off" class="w-4.5 h-4.5"></i>`;
            } else {
                pwdInput.type = 'password';
                if (eyeIcon) eyeIcon.innerHTML = `<i data-lucide="eye" class="w-4.5 h-4.5"></i>`;
            }
            lucide.createIcons();
        }
    };

    window.showLoginInterface = function() {
        window.playSynthesizedSFX('clean-pop');
        state.showLoginPanel = true;
        renderApp();
    };

    window.attemptPrivateLogin = function(e) {
        e.preventDefault();
        const userInput = document.getElementById('login-user-field').value.trim().toLowerCase();
        const typedPass = document.getElementById('login-password-field').value.trim();
        
        const targetUser = MOCK_USERS.find(u => 
            (u.username.toLowerCase() === userInput || u.id.toLowerCase() === userInput) && 
            u.password === typedPass
        );
        
        if (targetUser) {
            state.currentUser = targetUser;
            state.welcomeSessionActive = false;
            state.showLoginPanel = false;
            
            window.showToast(`Selamat datang, ${state.currentUser.name}!`, 'success');
            renderApp();
        } else {
            window.showToast("Username / sandi salah! Silakan periksa kembali.", "error");
        }
    };

    window.backToWelcomeScreen = function() {
        state.welcomeSessionActive = true;
        state.showLoginPanel = false;
        state.currentUser = null;
        state.impersonatedRole = null;
        renderApp();
    };

    window.setImpersonatedRole = function(role) {
        const hasAccess = state.currentUser && (state.currentUser.role === 'Director' || state.currentUser.role === 'Senior Editor');
        if (!hasAccess) {
            window.showToast('Anda tidak memiliki akses fitur ini.', 'error');
            return;
        }
        state.impersonatedRole = role === 'all' ? null : role;
        renderApp();
    };

    window.handleLogout = function() {
        state.currentUser = null;
        state.impersonatedRole = null;
        state.activeClientId = null;
        state.welcomeSessionActive = true; 
        state.showLoginPanel = false;
        window.showToast('Anda telah keluar dari Workspace.', 'success');
        renderApp();
    };

    window.selectClient = function(id) {
        state.activeClientId = id;
        state.sidebarActiveTab = 'dashboard';
        state.mobileSidebarOpen = false; 
        renderApp();
    };

    window.setFormatTab = function(tabName) {
        state.activeTab = tabName;
        window.playSynthesizedSFX('pop');
        renderApp();
    };

    window.setSidebarTab = function(tabName) {
        state.sidebarActiveTab = tabName;
        state.mobileSidebarOpen = false; 
        renderApp();
    };

    window.setSettingsTab = function(tabName) {
        state.settingsActiveTab = tabName;
        renderApp();
    };

    window.toggleNewClientModal = function(show) {
        state.showNewClientModal = show;
        renderApp();
    };

    window.createNewClient = async function(e) {
        e.preventDefault();
        const name = document.getElementById('new-client-name').value.trim();
        const editor = document.getElementById('new-client-editor').value;
        const logoUrl = document.getElementById('new-client-logo').value.trim() || 'https://placehold.co/150x150/bae2fd/0e93eb?text=' + encodeURIComponent(name[0]);

        if (!name) return;

        const newClient = {
            id: 'client-' + Date.now(),
            name: name,
            logo: logoUrl,
            assignedEditor: editor,
            colorPalette: [],
            graphicElements: [],
            fonts: [],
            guidelineSlides: [
                { id: 'slide-new-' + Date.now(), imageUrl: 'https://images.unsplash.com/photo-1611162617213-7d7a39e9b1d7?auto=format&fit=crop&w=800&q=80', text: 'Slide Utama: Letakkan identitas klien secara simetris.' }
            ],
            short: createEmptyTab('short'),
            long: createEmptyTab('long'),
            carousel: createEmptyTab('carousel')
        };

        if (isFirebaseOnline && db) {
            try {
                await setDoc(doc(db, 'artifacts', appId, 'public', 'data', 'clients', newClient.id), newClient);
                window.showToast('Klien baru berhasil ditambahkan!', 'success');
            } catch (err) {
                state.clients.push(newClient);
                saveLocalBackupIfOffline();
            }
        } else {
            state.clients.push(newClient);
            saveLocalBackupIfOffline();
            window.showToast('Klien baru ditambahkan ke penyimpanan lokal.', 'success');
        }

        state.activeClientId = newClient.id;
        state.showNewClientModal = false;
        renderApp();
    };

    window.handleClientLogoUpload = function(event, clientId) {
        const file = event.target.files[0];
        if (!file) return;

        const reader = new FileReader();
        reader.onload = async function(e) {
            const client = state.clients.find(c => c.id === clientId);
            if (client) {
                client.logo = e.target.result;
                await window.updateClientState(client);
                window.showToast("Foto profil klien berhasil diubah!", "success");
            }
        };
        reader.readAsDataURL(file);
    };

    window.updateClientState = async function(updatedClient) {
        const index = state.clients.findIndex(c => c.id === updatedClient.id);
        if (index !== -1) {
            state.clients[index] = updatedClient;
        }
        if (isFirebaseOnline && db) {
            try {
                await setDoc(doc(db, 'artifacts', appId, 'public', 'data', 'clients', updatedClient.id), updatedClient);
            } catch (err) {
                saveLocalBackupIfOffline();
            }
        } else {
            saveLocalBackupIfOffline();
        }
        renderApp();
    };

    window.addAssetItem = async function(category, item) {
        const client = state.clients.find(c => c.id === state.activeClientId);
        if (!client) return;

        if (category === 'colorPalette' || category === 'graphicElements' || category === 'fonts' || category === 'guidelineSlides') {
            if (!client[category]) {
                client[category] = [];
            }
            client[category].push(item);
        } else {
            const currentTab = state.activeTab;
            if (!client[currentTab]) {
                client[currentTab] = createEmptyTab(currentTab);
            }
            if (!client[currentTab][category]) {
                client[currentTab][category] = [];
            }
            client[currentTab][category].push(item);
        }
        await window.updateClientState(client);
    };

    window.deleteAssetItem = async function(category, itemId) {
        const client = state.clients.find(c => c.id === state.activeClientId);
        if (!client) return;

        if (category === 'colorPalette' || category === 'graphicElements' || category === 'fonts' || category === 'guidelineSlides') {
            if (client[category]) {
                client[category] = client[category].filter(item => item.id !== itemId);
            }
        } else {
            const currentTab = state.activeTab;
            if (client[currentTab] && client[currentTab][category]) {
                client[currentTab][category] = client[currentTab][category].filter(item => item.id !== itemId);
            }
        }
        await window.updateClientState(client);
        window.showToast('Item berhasil dihapus!', 'success');
    };

    window.updateClientField = async function(fieldName, value) {
        const client = state.clients.find(c => c.id === state.activeClientId);
        if (!client) return;

        if (fieldName === 'assignedEditor') {
            client.assignedEditor = value;
        } else if (fieldName === 'description') {
            client[state.activeTab].description = value;
        }
        await window.updateClientState(client);
    };

    window.handleAssetUpload = function(event, category) {
        const file = event.target.files[0];
        if (!file) return;

        const titleInput = document.getElementById(`upload-title-${category}`);
        const descInput = document.getElementById(`upload-desc-${category}`);
        
        const titleVal = titleInput ? titleInput.value.trim() : '';
        const descVal = descInput ? descInput.value.trim() : '';

        const reader = new FileReader();
        const feedback = document.getElementById(`${category}-upload-feedback`);
        if (feedback) {
            feedback.innerText = "Mengunggah... ⚡";
            feedback.className = "text-xs font-bold text-brand-500 animate-pulse";
        }

        reader.onload = async function(e) {
            const dataUrl = e.target.result;
            const newItem = {
                id: 'asset-' + Date.now(),
                name: file.name,
                url: dataUrl,
                title: titleVal || file.name,
                description: descVal || ''
            };

            if (category === 'fonts') {
                await window.addAssetItem('fonts', newItem);
                window.showToast(`Typeface ${file.name} berhasil ditambahkan!`, 'success');
            } else if (category === 'graphicElements') {
                await window.addAssetItem('graphicElements', newItem);
                window.showToast(`Elemen Grafis ${file.name} ditambahkan!`, 'success');
            } else if (category === 'transitions') {
                await window.addAssetItem('transitions', newItem);
                window.showToast(`Transisi ${file.name} ditambahkan!`, 'success');
            } else if (category === 'sfx') {
                const types = ['whoosh', 'ding', 'pop', 'swoosh'];
                const randomType = types[Math.floor(Math.random() * types.length)];
                await window.addAssetItem('sfx', { id: newItem.id, name: file.name, type: randomType, url: dataUrl });
                window.showToast(`SFX ${file.name} ditambahkan!`, 'success');
            }

            if (feedback) feedback.innerText = "";
            if (titleInput) titleInput.value = '';
            if (descInput) descInput.value = '';
        };

        if (file.size > 15 * 1024 * 1024) {
            window.showToast("File terlalu besar! Batasan maksimal file adalah 15MB.", "error");
            if (feedback) feedback.innerText = "";
            return;
        }
        reader.readAsDataURL(file);
    };

    window.addCustomLink = async function(e) {
        e.preventDefault();
        const title = document.getElementById('new-link-title').value.trim();
        const url = document.getElementById('new-link-url').value.trim();

        if (!title || !url) return;

        const newItem = {
            id: 'link-' + Date.now(),
            title: title,
            url: url
        };

        await window.addAssetItem('links', newItem);
        document.getElementById('new-link-title').value = '';
        document.getElementById('new-link-url').value = '';
        window.showToast('Link referensi ditambahkan!', 'success');
    };

    window.addGuidelineSlide = async function(e) {
        e.preventDefault();
        const client = state.clients.find(c => c.id === state.activeClientId);
        if (!client) return;

        const text = document.getElementById('new-gslide-text').value.trim();
        const fileInput = document.getElementById('new-gslide-image');
        const file = fileInput.files[0];

        if (!text) return;

        const performAdd = async (imageUrl) => {
            if (!client.guidelineSlides) {
                client.guidelineSlides = [];
            }
            client.guidelineSlides.push({
                id: 'gslide-' + Date.now(),
                imageUrl: imageUrl || 'https://images.unsplash.com/photo-1611162617213-7d7a39e9b1d7?auto=format&fit=crop&w=800&q=80',
                text: text
            });
            await window.updateClientState(client);
            document.getElementById('new-gslide-text').value = '';
            fileInput.value = '';
            window.showToast('Slide Guideline berhasil ditambahkan!', 'success');
        };

        if (file) {
            const reader = new FileReader();
            reader.onload = async function(evt) {
                await performAdd(evt.target.result);
            };
            reader.readAsDataURL(file);
        } else {
            await performAdd('');
        }
    };

    window.deleteGuidelineSlide = async function(slideId) {
        const client = state.clients.find(c => c.id === state.activeClientId);
        if (!client) return;

        client.guidelineSlides = client.guidelineSlides.filter(s => s.id !== slideId);
        state.activeSlideIndexes[client.id] = 0;
        
        await window.updateClientState(client);
        window.showToast('Slide Guideline dihapus.', 'success');
    };

    window.addContohOutputVideo = async function(e) {
        e.preventDefault();
        const client = state.clients.find(c => c.id === state.activeClientId);
        if (!client) return;

        const currentTab = state.activeTab;
        
        if (currentTab === 'long') {
            const note = document.getElementById('new-video-note').value.trim();
            const subCategory = document.getElementById('new-video-subcat').value;
            const fileInput = document.getElementById('new-video-file');
            const file = fileInput.files[0];

            if (!file) {
                window.showToast("Pilih file video terlebih dahulu!", "error");
                return;
            }

            const reader = new FileReader();
            reader.onload = async function(evt) {
                if (!client[currentTab].contohOutput) {
                    client[currentTab].contohOutput = [];
                }
                client[currentTab].contohOutput.push({
                    id: 'co-' + Date.now(),
                    name: file.name,
                    url: evt.target.result,
                    note: note || 'Tidak ada catatan.',
                    subCategory: subCategory
                });
                await window.updateClientState(client);
                document.getElementById('new-video-note').value = '';
                fileInput.value = '';
                window.showToast('Contoh Output video ditambahkan!', 'success');
            };
            reader.readAsDataURL(file);
        } else if (currentTab === 'short') {
            const title = document.getElementById('new-video-title-short').value.trim();
            const desc = document.getElementById('new-video-desc-short').value.trim();
            const fileInput = document.getElementById('new-video-file-short');
            const file = fileInput.files[0];

            if (!file) {
                window.showToast("Pilih file video terlebih dahulu!", "error");
                return;
            }

            const reader = new FileReader();
            reader.onload = async function(evt) {
                if (!client[currentTab].contohOutput) {
                    client[currentTab].contohOutput = [];
                }
                client[currentTab].contohOutput.push({
                    id: 'co-sh-' + Date.now(),
                    title: title || file.name,
                    description: desc || 'Tidak ada keterangan.',
                    url: evt.target.result,
                    name: file.name
                });
                await window.updateClientState(client);
                document.getElementById('new-video-title-short').value = '';
                document.getElementById('new-video-desc-short').value = '';
                fileInput.value = '';
                window.showToast('Video Short 9:16 berhasil ditambahkan!', 'success');
            };
            reader.readAsDataURL(file);
        } else if (currentTab === 'carousel') {
            const title = document.getElementById('new-img-title-carousel').value.trim();
            const desc = document.getElementById('new-img-desc-carousel').value.trim();
            const fileInput = document.getElementById('new-img-file-carousel');
            const file = fileInput.files[0];

            if (!file) {
                window.showToast("Pilih file gambar terlebih dahulu!", "error");
                return;
            }

            const reader = new FileReader();
            reader.onload = async function(evt) {
                if (!client[currentTab].contohOutput) {
                    client[currentTab].contohOutput = [];
                }
                client[currentTab].contohOutput.push({
                    id: 'co-car-' + Date.now(),
                    title: title || file.name,
                    description: desc || 'Tidak ada keterangan.',
                    url: evt.target.result,
                    name: file.name
                });
                await window.updateClientState(client);
                document.getElementById('new-img-title-carousel').value = '';
                document.getElementById('new-img-desc-carousel').value = '';
                fileInput.value = '';
                window.showToast('Gambar Carousel 4:5 berhasil ditambahkan!', 'success');
            };
            reader.readAsDataURL(file);
        }
    };

    window.deleteContohOutputVideo = async function(videoId) {
        const client = state.clients.find(c => c.id === state.activeClientId);
        if (!client) return;

        const currentTab = state.activeTab;
        client[currentTab].contohOutput = client[currentTab].contohOutput.filter(v => v.id !== videoId);
        await window.updateClientState(client);
        window.showToast('Contoh Output berhasil dihapus.', 'success');
    };

    window.addColorPaletteItem = async function(e) {
        e.preventDefault();
        const name = document.getElementById('new-color-name').value.trim() || 'Custom Accent';
        const hex = document.getElementById('new-color-hex').value.trim();

        if (!hex.startsWith('#') || hex.length < 4) {
            window.showToast("Gunakan format hex warna valid (Cth: #FF3E6C)", "error");
            return;
        }

        const newItem = {
            id: 'col-' + Date.now(),
            name: name,
            hex: hex
        };

        await window.addAssetItem('colorPalette', newItem);
        document.getElementById('new-color-name').value = '';
        document.getElementById('new-color-hex').value = '';
        window.showToast('Palet warna ditambahkan!', 'success');
    };

    window.changeSlideIndex = function(clientId, direction, maxSlides) {
        if (state.activeSlideIndexes[clientId] === undefined) {
            state.activeSlideIndexes[clientId] = 0;
        }
        let currentIndex = state.activeSlideIndexes[clientId];
        currentIndex += direction;
        if (currentIndex < 0) currentIndex = maxSlides - 1;
        if (currentIndex >= maxSlides) currentIndex = 0;
        
        state.activeSlideIndexes[clientId] = currentIndex;
        window.playSynthesizedSFX('whoosh');
        renderApp();
    };

    // User explicitly paused slides
    window.manuallyPauseAutoplay = function(clientId) {
        state.autoplayPaused[clientId] = true;
        window.showToast("Autoplay slide dijeda sementara.", "success");
        renderApp();
    };

    window.changeVideoCarouselIndex = function(clientId, tabName, subCategory, direction, maxVideos) {
        const stateKey = `${clientId}-${tabName}-${subCategory}`;
        if (state.activeVideoIndexes[stateKey] === undefined) {
            state.activeVideoIndexes[stateKey] = 0;
        }
        let currentIndex = state.activeVideoIndexes[stateKey];
        currentIndex += direction;
        if (currentIndex < 0) currentIndex = maxVideos - 1;
        if (currentIndex >= maxVideos) currentIndex = 0;
        
        state.activeVideoIndexes[stateKey] = currentIndex;
        window.playSynthesizedSFX('swoosh');
        renderApp();
    };

    window.saveProfileSettings = function(e) {
        e.preventDefault();
        const dispName = document.getElementById('settings-display-name').value.trim();
        const username = document.getElementById('settings-username').value.trim();
        
        if (dispName && username) {
            state.currentUser.name = dispName;
            state.currentUser.username = username;
            
            const userIdx = MOCK_USERS.findIndex(u => u.id === state.currentUser.id);
            if (userIdx !== -1) {
                MOCK_USERS[userIdx].name = dispName;
                MOCK_USERS[userIdx].username = username;
                saveUsersToLocalStorage();
            }
            
            window.showToast("Pengaturan profil berhasil disimpan!", "success");
            renderApp();
        }
    };

    window.handlePasswordChangeSubmit = function(e) {
        if (e) e.preventDefault();
        const currentPass = document.getElementById('settings-current-password').value;
        const newPass = document.getElementById('settings-new-password').value;

        if (!currentPass || !newPass) {
            window.showToast("Semua kolom harus diisi!", "error");
            return;
        }

        const userIdx = MOCK_USERS.findIndex(u => u.id === state.currentUser.id);
        if (userIdx !== -1) {
            if (MOCK_USERS[userIdx].password === currentPass) {
                MOCK_USERS[userIdx].password = newPass;
                state.currentUser.password = newPass;
                saveUsersToLocalStorage();
                
                document.getElementById('settings-current-password').value = '';
                document.getElementById('settings-new-password').value = '';
                window.showToast("Kata sandi berhasil diubah secara aman!", "success");
                renderApp();
            } else {
                window.showToast("Kata sandi saat ini salah!", "error");
            }
        }
    };

    function getFilteredClients() {
        const user = state.currentUser;
        if (!user) return [];
        
        const activeRole = state.impersonatedRole || user.role;
        
        if (user.role === 'Director' || user.role === 'Senior Editor') {
            if (state.impersonatedRole) {
                return state.clients.filter(c => c.assignedEditor === state.impersonatedRole);
            }
            return state.clients;
        }
        
        return state.clients.filter(c => c.assignedEditor === user.role);
    }

    function getSocialIcon(url) {
        if (!url) return '';
        const lower = url.toLowerCase();
        if (lower.includes('instagram.com')) {
            return `
                <span class="inline-flex items-center justify-center w-8 h-8 rounded-xl bg-gradient-to-tr from-yellow-500 via-red-500 to-purple-600 text-white shadow-md mr-2 shrink-0" title="Instagram Link">
                    <svg class="w-4.5 h-4.5 fill-current" viewBox="0 0 24 24">
                        <path d="M12 2.163c3.204 0 3.584.012 4.85.07 3.252.148 4.771 1.691 4.919 4.919.058 1.265.069 1.645.069 4.849 0 3.205-.012 3.584-.069 4.849-.149 3.225-1.664 4.771-4.919 4.919-1.266.058-1.644.07-4.85.07-3.204 0-3.584-.012-4.849-.07-3.26-.149-4.771-1.699-4.919-4.92-.058-1.265-.07-1.644-.07-4.849 0-3.204.013-3.583.07-4.849.149-3.227 1.664-4.771 4.919-4.919 1.266-.057 1.645-.069 4.849-.069zM12 0C8.741 0 8.333.014 7.053.072 2.695.272.273 2.69.073 7.051.014 8.333 0 8.741 0 12c0 3.259.014 3.668.072 4.948.2 4.358 2.618 6.78 6.98 6.98 1.281.058 1.689.072 4.948.072 3.259 0 3.668-.014 4.948-.072 4.354-.2 6.782-2.618 6.979-6.98.059-1.28.073-1.689.073-4.948 0-3.259-.014-3.667-.072-4.947-.196-4.354-2.617-6.78-6.979-6.98C15.668.014 15.259 0 12 0zm0 5.838a6.162 6.162 0 100 12.324 6.162 6.162 0 000-12.324zM12 16a4 4 0 110-8 4 4 0 010 8zm6.406-11.845a1.44 1.44 0 100 2.881 1.44 1.44 0 000-2.881z"/>
                    </svg>
                </span>
            `;
        } else if (lower.includes('tiktok.com')) {
            return `
                <span class="inline-flex items-center justify-center w-8 h-8 rounded-xl bg-black text-white shadow-md mr-2 shrink-0" title="TikTok Link">
                    <svg class="w-4.5 h-4.5 fill-current" viewBox="0 0 24 24">
                        <path d="M12.525.02c1.31-.02 2.61-.01 3.91-.02.08 1.53.63 3.02 1.59 4.23.97 1.21 2.34 2.11 3.86 2.58v4.03c-1.48-.17-2.91-.76-4.13-1.72-.45-.35-.86-.76-1.22-1.22v7.19c.12 3.16-1.57 6.17-4.43 7.59-2.86 1.42-6.37 1.14-8.96-.73-2.58-1.87-3.87-5.18-3.24-8.34.63-3.17 3.19-5.69 6.4-6.31v4.06c-1.7.35-3.04 1.76-3.23 3.49-.25 2.17 1.29 4.14 3.47 4.41 2.18.27 4.15-1.27 4.43-3.45.05-.41.06-.83.02-1.24V.02z"/>
                    </svg>
                </span>
            `;
        } else {
            return `
                <span class="inline-flex items-center justify-center w-8 h-8 rounded-xl bg-brand-100 dark:bg-brand-900 text-brand-600 dark:text-brand-300 mr-2 shrink-0" title="External Link">
                    <svg class="w-4.5 h-4.5" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M13.828 10.172a4 4 0 00-5.656 0l-4 4a4 4 0 105.656 5.656l1.102-1.101m-.758-4.899a4 4 0 005.656 0l4-4a4 4 0 00-5.656-5.656l-1.1 1.1"/></svg>
                </span>
            `;
        }
    }

    window.renderApp = function() {
        const root = document.getElementById('app-root');
        
        if (state.isLoading) {
            root.innerHTML = `
                <div class="flex flex-col items-center justify-center min-h-screen">
                    <div class="w-16 h-16 border-4 border-brand-200 border-t-brand-500 rounded-full animate-spin"></div>
                    <p class="mt-4 text-brand-700 font-semibold tracking-wide">Menghubungkan ke Cloud Agency...</p>
                </div>
            `;
            return;
        }

        // Render Welcome Splash Screen
        if (state.welcomeSessionActive && !state.currentUser) {
            renderWelcomeSplashPage(root);
            return;
        }

        const filteredClients = getFilteredClients();
        const activeClient = state.clients.find(c => c.id === state.activeClientId) || filteredClients[0];
        
        if (filteredClients.length > 0 && (!state.activeClientId || !state.clients.some(c => c.id === state.activeClientId))) {
            state.activeClientId = filteredClients[0].id;
        }

        const isSenior = state.currentUser.role === 'Senior Editor';
        const isDirector = state.currentUser.role === 'Director';
        const canEdit = isSenior; 

        root.innerHTML = `
            <div class="min-h-screen flex bg-slate-50 dark:bg-slate-900 transition-colors duration-300 font-sans">
                
                <!-- Collapsible Left Sidebar echoing image_3e3814.png -->
                <aside class="${state.sidebarCollapsed ? 'w-20' : 'w-72'} hidden md:flex bg-white dark:bg-slate-950 border-r border-slate-200/80 dark:border-slate-800/80 shrink-0 flex-col justify-between py-6 transition-all duration-300 z-35">
                    <div>
                        <!-- Brand Header -->
                        <div class="flex items-center gap-3 px-6 pb-6 border-b border-slate-100 dark:border-slate-800/80">
                            <div class="w-10 h-10 rounded-xl bg-gradient-to-tr from-brand-400 to-brand-600 flex items-center justify-center shadow-md text-white shrink-0">
                                <i data-lucide="video" class="w-5.5 h-5.5"></i>
                            </div>
                            <div class="overflow-hidden whitespace-nowrap transition-all ${state.sidebarCollapsed ? 'opacity-0 w-0' : 'opacity-100 w-auto'}">
                                <h1 class="font-extrabold text-slate-800 dark:text-white text-md tracking-tight">ClientGuide</h1>
                                <p class="text-[9px] text-brand-500 font-extrabold tracking-widest uppercase">Workspace</p>
                            </div>
                        </div>

                        <!-- Sidebar Menu Items -->
                        <nav class="mt-6 px-4 flex flex-col gap-1.5">
                            <button onclick="setSidebarTab('dashboard')" class="w-full flex items-center gap-3 px-4 py-3 rounded-2xl font-bold text-xs transition-all ${state.sidebarActiveTab === 'dashboard' ? 'bg-brand-100 text-brand-700 dark:bg-brand-900/40 dark:text-brand-300' : 'text-slate-600 dark:text-slate-400 hover:bg-slate-100 dark:hover:bg-slate-800/50'}">
                                <i data-lucide="layout-dashboard" class="w-5 h-5 shrink-0"></i>
                                <span class="overflow-hidden whitespace-nowrap ${state.sidebarCollapsed ? 'opacity-0 w-0' : 'opacity-100 w-auto'}">Dashboard</span>
                            </button>
                            
                            <button onclick="setSidebarTab('clients')" class="w-full flex items-center gap-3 px-4 py-3 rounded-2xl font-bold text-xs transition-all ${state.sidebarActiveTab === 'clients' ? 'bg-brand-100 text-brand-700 dark:bg-brand-900/40 dark:text-brand-300' : 'text-slate-600 dark:text-slate-400 hover:bg-slate-100 dark:hover:bg-slate-800/50'}">
                                <i data-lucide="folder-git" class="w-5 h-5 shrink-0"></i>
                                <span class="overflow-hidden whitespace-nowrap ${state.sidebarCollapsed ? 'opacity-0 w-0' : 'opacity-100 w-auto'}">Semua Klien</span>
                            </button>

                            <button onclick="setSidebarTab('settings')" class="w-full flex items-center gap-3 px-4 py-3 rounded-2xl font-bold text-xs transition-all ${state.sidebarActiveTab === 'settings' ? 'bg-brand-100 text-brand-700 dark:bg-brand-900/40 dark:text-brand-300' : 'text-slate-600 dark:text-slate-400 hover:bg-slate-100 dark:hover:bg-slate-800/50'}">
                                <i data-lucide="settings" class="w-5 h-5 shrink-0"></i>
                                <span class="overflow-hidden whitespace-nowrap ${state.sidebarCollapsed ? 'opacity-0 w-0' : 'opacity-100 w-auto'}">Settings</span>
                            </button>
                        </nav>

                        <!-- Client Quick Nav within sidebar -->
                        <div class="mt-8 px-6 ${state.sidebarCollapsed ? 'hidden' : 'block'}">
                            <p class="text-[10px] font-extrabold uppercase text-slate-400 tracking-wider mb-2">Penugasan Klien Anda</p>
                            <div class="flex flex-col gap-1 overflow-y-auto max-h-[220px] pr-2">
                                ${filteredClients.map(c => `
                                    <button onclick="selectClient('${c.id}')" class="w-full text-left px-3 py-2 rounded-xl text-xs font-bold truncate transition-all ${state.activeClientId === c.id ? 'bg-brand-50 dark:bg-slate-900 text-brand-600 dark:text-brand-300' : 'text-slate-500 hover:bg-slate-50 dark:hover:bg-slate-850'}">
                                        • ${c.name}
                                    </button>
                                `).join('')}
                            </div>
                        </div>
                    </div>

                    <!-- Sidebar Footer area -->
                    <div class="px-4 flex flex-col gap-4">
                        <button onclick="toggleSidebar()" class="self-center p-2 rounded-xl bg-slate-100 hover:bg-slate-200 dark:bg-slate-800 dark:hover:bg-slate-700 text-slate-600 dark:text-slate-300 transition-all" title="Perlebar/Kecilkan Sidebar">
                            <i data-lucide="${state.sidebarCollapsed ? 'chevron-right' : 'chevron-left'}" class="w-4 h-4"></i>
                        </button>

                        <div class="bg-slate-50 dark:bg-slate-900/50 border border-slate-100 dark:border-slate-800 p-3.5 rounded-2xl flex items-center justify-between gap-2 overflow-hidden">
                            <div class="flex items-center gap-2 overflow-hidden">
                                <div class="w-8 h-8 rounded-full bg-brand-100 dark:bg-brand-900 text-brand-700 dark:text-brand-300 flex items-center justify-center font-bold text-sm shrink-0">
                                    ${state.currentUser.avatar}
                                </div>
                                <div class="text-left overflow-hidden whitespace-nowrap ${state.sidebarCollapsed ? 'hidden' : 'block'}">
                                    <p class="text-[11px] font-extrabold text-slate-700 dark:text-slate-200 truncate">${state.currentUser.name}</p>
                                    <p class="text-[9px] text-slate-400 font-semibold uppercase truncate">${state.currentUser.role}</p>
                                </div>
                            </div>
                            <button onclick="handleLogout()" class="text-rose-500 hover:text-rose-600 shrink-0 ${state.sidebarCollapsed ? 'mx-auto' : ''}">
                                <i data-lucide="log-out" class="w-4 h-4"></i>
                            </button>
                        </div>
                    </div>
                </aside>

                <!-- Mobile Navigation Drawer -->
                <div id="mobile-sidebar-drawer" class="fixed inset-0 z-50 bg-slate-900/60 backdrop-blur-sm md:hidden transition-opacity duration-300 ${state.mobileSidebarOpen ? 'opacity-100 pointer-events-auto' : 'opacity-0 pointer-events-none'}" onclick="toggleMobileSidebar()">
                    <div class="w-72 max-w-[80vw] h-full bg-white dark:bg-slate-950 p-5 flex flex-col justify-between transition-transform duration-300 transform ${state.mobileSidebarOpen ? 'translate-x-0' : '-translate-x-full'}" onclick="event.stopPropagation()">
                        <div>
                            <div class="flex items-center justify-between pb-4 border-b dark:border-slate-800">
                                <div class="flex items-center gap-2">
                                    <div class="w-8 h-8 rounded-lg bg-brand-500 text-white flex items-center justify-center shadow">
                                        <i data-lucide="video" class="w-4 h-4"></i>
                                    </div>
                                    <span class="font-bold text-sm">Workspace</span>
                                </div>
                                <button onclick="toggleMobileSidebar()" class="p-1.5 rounded-lg bg-slate-100 dark:bg-slate-800">
                                    <i data-lucide="x" class="w-4 h-4"></i>
                                </button>
                            </div>
                            <nav class="mt-6 flex flex-col gap-1.5">
                                <button onclick="setSidebarTab('dashboard')" class="w-full flex items-center gap-3 px-4 py-2.5 rounded-xl font-bold text-xs ${state.sidebarActiveTab === 'dashboard' ? 'bg-brand-100 text-brand-700 dark:bg-brand-900/40 dark:text-brand-300' : 'text-slate-600 hover:bg-slate-100'}">
                                    <i data-lucide="layout-dashboard" class="w-4 h-4"></i>
                                    Dashboard
                                </button>
                                <button onclick="setSidebarTab('clients')" class="w-full flex items-center gap-3 px-4 py-2.5 rounded-xl font-bold text-xs ${state.sidebarActiveTab === 'clients' ? 'bg-brand-100 text-brand-700 dark:bg-brand-900/40 dark:text-brand-300' : 'text-slate-600 hover:bg-slate-100'}">
                                    <i data-lucide="folder-git" class="w-4 h-4"></i>
                                    Semua Klien
                                </button>
                                <button onclick="setSidebarTab('settings')" class="w-full flex items-center gap-3 px-4 py-2.5 rounded-xl font-bold text-xs ${state.sidebarActiveTab === 'settings' ? 'bg-brand-100 text-brand-700 dark:bg-brand-900/40 dark:text-brand-300' : 'text-slate-600 hover:bg-slate-100'}">
                                    <i data-lucide="settings" class="w-4 h-4"></i>
                                    Settings
                                </button>
                            </nav>

                            <div class="mt-6">
                                <p class="text-[10px] font-extrabold uppercase text-slate-400 tracking-wider px-4 mb-2">Penugasan Klien Anda</p>
                                <div class="flex flex-col gap-1 px-2">
                                    ${filteredClients.map(c => `
                                        <button onclick="selectClient('${c.id}')" class="w-full text-left px-3 py-2 rounded-xl text-xs font-bold truncate ${state.activeClientId === c.id ? 'bg-brand-50 dark:bg-slate-800 text-brand-600' : 'text-slate-500'}">
                                            • ${c.name}
                                        </button>
                                    `).join('')}
                                </div>
                            </div>
                        </div>

                        <div class="border-t dark:border-slate-800 pt-4 flex flex-col gap-3">
                            <div class="flex items-center gap-2 px-2">
                                <div class="text-xs">
                                    <p class="font-extrabold">${state.currentUser.name}</p>
                                    <p class="text-[9px] uppercase text-slate-400 font-semibold">${state.currentUser.role}</p>
                                </div>
                            </div>
                            <button onclick="handleLogout()" class="w-full flex items-center justify-center gap-2 py-2.5 bg-rose-50 text-rose-600 dark:bg-rose-950/20 dark:text-rose-400 font-bold text-xs rounded-xl">
                                <i data-lucide="log-out" class="w-4 h-4"></i>
                                Logout
                            </button>
                        </div>
                    </div>
                </div>

                <div class="flex-1 flex flex-col min-h-screen overflow-x-hidden">
                    
                    <!-- Top Navigation Hub -->
                    <header class="glass-card sticky top-0 z-40 px-4 md:px-6 py-4 shadow-sm border-b border-slate-200/50 dark:border-slate-800/40 flex items-center justify-between gap-4">
                        <div class="flex items-center gap-2">
                            <!-- Hamburger Trigger on Mobile -->
                            <button onclick="toggleMobileSidebar()" class="md:hidden p-2 rounded-xl bg-slate-100 dark:bg-slate-800 hover:bg-slate-200 text-slate-700 dark:text-slate-300" title="Menu">
                                <i data-lucide="menu" class="w-5 h-5"></i>
                            </button>
                            
                            <!-- Theme Mode selection -->
                            <div class="flex items-center gap-1 bg-slate-100 dark:bg-slate-800 p-1 rounded-xl">
                                <button onclick="toggleDarkMode(false)" class="p-1.5 rounded-lg ${!state.darkMode ? 'bg-white text-amber-500 shadow-sm' : 'text-slate-400'}" title="Mode Terang">
                                    <i data-lucide="sun" class="w-3.5 h-3.5"></i>
                                </button>
                                <button onclick="toggleDarkMode(true)" class="p-1.5 rounded-lg ${state.darkMode ? 'bg-slate-700 text-blue-400 shadow-sm' : 'text-slate-400'}" title="Mode Gelap">
                                    <i data-lucide="moon" class="w-3.5 h-3.5"></i>
                                </button>
                            </div>
                        </div>

                        <!-- Impersonation Selector -->
                        ${(isSenior || isDirector) ? `
                            <div class="flex items-center gap-2 bg-brand-50 dark:bg-slate-850 border border-brand-100/50 dark:border-slate-800/50 p-1 rounded-xl">
                                <span class="hidden lg:inline-block text-[10px] uppercase font-extrabold text-brand-700 dark:text-brand-300 px-2">
                                    Tinjau Sebagai Editor:
                                </span>
                                <div class="flex gap-1">
                                    <button onclick="setImpersonatedRole('all')" class="px-2 py-1 text-[10px] font-bold rounded-lg transition-all ${!state.impersonatedRole ? 'bg-brand-500 text-white' : 'text-slate-600 dark:text-slate-300 hover:bg-white/40'}">
                                        Semua
                                    </button>
                                    <button onclick="setImpersonatedRole('Dina')" class="px-2 py-1 text-[10px] font-bold rounded-lg transition-all ${state.impersonatedRole === 'Dina' ? 'bg-brand-500 text-white' : 'text-slate-600 dark:text-slate-300 hover:bg-white/40'}">
                                        Dina
                                    </button>
                                    <button onclick="setImpersonatedRole('Nopi')" class="px-2 py-1 text-[10px] font-bold rounded-lg transition-all ${state.impersonatedRole === 'Nopi' ? 'bg-brand-500 text-white' : 'text-slate-600 dark:text-slate-300 hover:bg-white/40'}">
                                        Nopi
                                    </button>
                                    <button onclick="setImpersonatedRole('Diva')" class="px-2 py-1 text-[10px] font-bold rounded-lg transition-all ${state.impersonatedRole === 'Diva' ? 'bg-brand-500 text-white' : 'text-slate-600 dark:text-slate-300 hover:bg-white/40'}">
                                        Diva
                                    </button>
                                </div>
                            </div>
                        ` : ''}
                    </header>

                    <!-- Workspace View Render Area -->
                    <main class="flex-1 p-4 md:p-6">
                        ${renderActiveSidebarSection(activeClient, filteredClients, canEdit, isSenior)}
                    </main>

                </div>
            </div>

            <!-- Client Creation Modal -->
            ${state.showNewClientModal ? `
                <div class="fixed inset-0 bg-slate-900/40 backdrop-blur-sm flex items-center justify-center z-50 p-4">
                    <div class="bg-white dark:bg-slate-900 rounded-4xl w-full max-w-md shadow-2xl p-6 relative">
                        <button onclick="toggleNewClientModal(false)" class="absolute top-5 right-5 text-slate-400 hover:text-slate-600 p-1.5 rounded-xl hover:bg-slate-50 transition-all">
                            <i data-lucide="x" class="w-5 h-5"></i>
                        </button>
                        
                        <h3 class="font-extrabold text-slate-800 dark:text-white text-lg mb-4">Tambah Klien Personal Brand Baru</h3>
                        <form onsubmit="createNewClient(event)" class="flex flex-col gap-4">
                            <div>
                                <label class="text-xs font-bold text-slate-500 block mb-1">Nama Brand / Tokoh</label>
                                <input type="text" id="new-client-name" required placeholder="Cth: Merry Riana Brand" class="w-full bg-slate-50 dark:bg-slate-800 border border-slate-200 dark:border-slate-700 rounded-xl p-3 text-sm focus:outline-none focus:ring-2 focus:ring-brand-200 transition-all">
                            </div>
                            
                            <div>
                                <label class="text-xs font-bold text-slate-500 block mb-1">Editor Penanggung Jawab</label>
                                <select id="new-client-editor" class="w-full bg-slate-50 dark:bg-slate-800 border border-slate-200 dark:border-slate-700 rounded-xl p-3 text-sm font-semibold text-slate-700 dark:text-slate-200 focus:outline-none focus:ring-2 focus:ring-brand-200 transition-all">
                                    <option value="Dina">Dina</option>
                                    <option value="Nopi">Nopi</option>
                                    <option value="Diva">Diva</option>
                                </select>
                            </div>
                            
                            <div>
                                <label class="text-xs font-bold text-slate-500 block mb-1">Logo / Foto URL (Opsional)</label>
                                <input type="url" id="new-client-logo" placeholder="https://images.unsplash.com/..." class="w-full bg-slate-50 dark:bg-slate-800 border border-slate-200 dark:border-slate-700 rounded-xl p-3 text-sm focus:outline-none focus:ring-2 focus:ring-brand-200 transition-all">
                            </div>

                            <button type="submit" class="w-full bg-brand-500 hover:bg-brand-600 text-white rounded-2xl py-3.5 font-bold text-sm tracking-wide mt-2 shadow-lg shadow-brand-100 transition-all">
                                Daftarkan Klien
                            </button>
                        </form>
                    </div>
                </div>
            ` : ''}

            <!-- Custom Delete Client Confirmation Modal -->
            ${state.clientToDeleteId ? `
                <div class="fixed inset-0 bg-slate-900/50 backdrop-blur-sm flex items-center justify-center z-50 p-4">
                    <div class="bg-white dark:bg-slate-900 rounded-3xl w-full max-w-sm shadow-2xl p-6 text-center border border-slate-100 dark:border-slate-800 animate-in fade-in zoom-in-95 duration-200">
                        <div class="w-12 h-12 rounded-full bg-rose-50 dark:bg-rose-950/30 text-rose-500 flex items-center justify-center mx-auto mb-4">
                            <i data-lucide="alert-triangle" class="w-6 h-6"></i>
                        </div>
                        <h3 class="font-extrabold text-slate-800 dark:text-white text-md mb-2">Hapus Klien</h3>
                        <p class="text-xs text-slate-500 dark:text-slate-400 mb-6">Apakah Anda yakin ingin menghapus klien ini? Seluruh data guideline, aset, dan video acuan akan terhapus permanen.</p>
                        <div class="flex gap-3">
                            <button onclick="window.cancelDeleteClient()" class="flex-1 py-3 bg-slate-100 hover:bg-slate-200 dark:bg-slate-800 dark:hover:bg-slate-700 text-slate-700 dark:text-slate-200 rounded-2xl font-bold text-xs transition-all">
                                Batal
                            </button>
                            <button onclick="window.executeDeleteClient()" class="flex-1 py-3 bg-rose-500 hover:bg-rose-600 text-white rounded-2xl font-bold text-xs transition-all shadow-lg shadow-rose-100 dark:shadow-none">
                                Ya, Hapus
                            </button>
                        </div>
                    </div>
                </div>
            ` : ''}
        `;
        lucide.createIcons();
    };

    function renderWelcomeSplashPage(root) {
        const radius = 110;
        
        // Abstract anonymous placeholders to keep privacy
        const itemsData = [
            { id: '1', emoji: '👑', color: 'from-amber-200 to-yellow-400' },
            { id: '2', emoji: '⚡', color: 'from-blue-200 to-blue-500' },
            { id: '3', emoji: '✍️', color: 'from-pink-200 to-rose-400' },
            { id: '4', emoji: '🎬', color: 'from-emerald-200 to-teal-500' },
            { id: '5', emoji: '🎨', color: 'from-purple-200 to-indigo-500' }
        ];

        let orbitItemsHTML = '';
        itemsData.forEach((item, index) => {
            const angleDeg = index * 72; 
            const angleRad = (angleDeg * Math.PI) / 180;
            const x = radius * Math.cos(angleRad);
            const y = radius * Math.sin(angleRad);
            
            orbitItemsHTML += `
                <div class="orbit-item flex flex-col items-center justify-center select-none" 
                     style="transform: translate(${x}px, ${y}px);">
                    <div class="orbit-inner-face w-14 h-14 md:w-16 md:h-16 rounded-full bg-gradient-to-tr ${item.color} flex items-center justify-center text-2xl md:text-3xl shadow-lg border border-white/60 dark:border-slate-800/40 relative group cursor-default">
                         ${item.emoji}
                         <div class="absolute inset-0 rounded-full bg-white opacity-0 group-hover:opacity-10 transition-opacity"></div>
                    </div>
                </div>
            `;
        });

        if (!state.showLoginPanel) {
            root.innerHTML = `
                <div class="min-h-screen flex flex-col items-center justify-center p-6 text-center select-none">
                    <div class="w-full max-w-lg flex flex-col items-center gap-8 md:gap-10">
                        
                        <!-- 1. Interactive Orbit Wheel -->
                        <div class="relative w-72 h-72 md:w-80 md:h-80 flex items-center justify-center mt-6">
                            <div class="absolute w-52 h-52 bg-brand-200/40 dark:bg-brand-900/10 rounded-full blur-3xl animate-pulse pointer-events-none"></div>
                            <div class="absolute w-[220px] h-[220px] rounded-full border border-slate-200/50 dark:border-slate-800/40 pointer-events-none"></div>
                            <div class="absolute w-[140px] h-[140px] rounded-full border border-dashed border-slate-200/60 dark:border-slate-800/40 pointer-events-none"></div>

                            <!-- Main revolving ring of Memoji icons -->
                            <div id="orbit-ring-rotator" class="absolute w-full h-full" style="transform: rotate(${state.welcomeOrbitAngle}deg); transition: transform 1.1s cubic-bezier(0.25, 1, 0.5, 1);">
                                ${orbitItemsHTML}
                            </div>

                            <!-- Central Cewek dengan Laptop (Woman Technologist) Emoji -->
                            <div class="absolute w-20 h-20 md:w-24 md:h-24 rounded-full bg-white dark:bg-slate-900 shadow-xl border-2 border-brand-300 dark:border-slate-700 flex items-center justify-center overflow-hidden z-10 p-1">
                                <span class="text-4xl md:text-5xl select-none animate-bounce">👩‍💻</span>
                            </div>
                        </div>

                        <!-- 2. Typography Headings -->
                        <div class="flex flex-col gap-2">
                            <h1 class="font-bold text-2xl md:text-3.5xl text-slate-900 dark:text-white tracking-tight leading-tight">
                                Ready to create some masterpieces?
                            </h1>
                            <p class="text-xs md:text-sm text-brand-600 dark:text-brand-400 font-medium tracking-wide">
                                Your timeline is waiting!
                            </p>
                        </div>

                        <!-- 3. Minimalist Pro Let's Go Trigger Button -->
                        <button onclick="showLoginInterface()" class="group px-8 py-3 bg-slate-900 hover:bg-brand-600 dark:bg-slate-800 dark:hover:bg-brand-600 text-white font-semibold text-xs tracking-wider uppercase rounded-xl transition-all duration-300 flex items-center gap-2">
                            LET'S GO!
                            <i data-lucide="chevron-right" class="w-3.5 h-3.5 group-hover:translate-x-1 transition-transform"></i>
                        </button>

                    </div>
                </div>
            `;
        } else {
            // Direct secure credentials login interface matching WhatsApp Image 2026-07-12 at 10.34.11.jpeg
            root.innerHTML = `
                <div class="min-h-screen flex items-center justify-center p-6 bg-gradient-to-b from-sky-50 to-white dark:from-slate-950 dark:to-slate-900">
                    <div class="w-full max-w-sm bg-white/90 dark:bg-slate-900/90 backdrop-blur-2xl border border-slate-200/60 dark:border-slate-800/50 p-6 md:p-8 rounded-[2rem] shadow-2xl flex flex-col gap-6 relative transition-all">
                        
                        <!-- Back button matching layout in reference photo -->
                        <button onclick="backToWelcomeScreen()" class="absolute top-6 left-6 text-slate-400 hover:text-slate-600 font-semibold text-xs flex items-center gap-1 transition-all">
                            <i data-lucide="chevron-left" class="w-4 h-4"></i>
                            Kembali
                        </button>

                        <div class="text-center mt-6 flex flex-col items-center">
                            <!-- Secure Lock Avatar Container -->
                            <div class="w-16 h-16 rounded-full bg-brand-50 border border-brand-200 flex items-center justify-center text-brand-500 mb-3 shadow-inner">
                                <i data-lucide="shield-check" class="w-8 h-8"></i>
                            </div>
                            <h2 class="font-extrabold text-base text-slate-800 dark:text-white uppercase tracking-wider">Akses Workspace</h2>
                            <p class="text-[10px] text-slate-400 font-semibold mt-1">Gunakan kredensial terdaftar untuk masuk</p>
                        </div>

                        <form onsubmit="attemptPrivateLogin(event)" class="flex flex-col gap-5">
                            
                            <!-- Username Field -->
                            <div class="flex flex-col gap-1.5">
                                <label class="block text-[10px] font-extrabold text-slate-400 uppercase tracking-wider">Username atau Email</label>
                                <div class="relative flex items-center">
                                    <span class="absolute left-3.5 text-slate-400">
                                        <i data-lucide="user" class="w-4 h-4"></i>
                                    </span>
                                    <input 
                                        type="text" 
                                        id="login-user-field" 
                                        required 
                                        placeholder="nama@agency." 
                                        class="w-full bg-slate-50 dark:bg-slate-800 border border-slate-200 dark:border-slate-700 rounded-2xl pl-10 pr-4 py-3 text-sm focus:outline-none focus:ring-2 focus:ring-brand-200/50 text-slate-700 dark:text-slate-150 font-medium tracking-wide"
                                    >
                                </div>
                            </div>

                            <!-- Password Input with dynamic eye visibility toggle -->
                            <div class="flex flex-col gap-1.5">
                                <label class="block text-[10px] font-extrabold text-slate-400 uppercase tracking-wider">Masukkan Kata Sandi</label>
                                <div class="relative flex items-center">
                                    <span class="absolute left-3.5 text-slate-400">
                                        <i data-lucide="lock" class="w-4 h-4"></i>
                                    </span>
                                    <input 
                                        type="password" 
                                        id="login-password-field" 
                                        required 
                                        placeholder="••••••••" 
                                        class="w-full bg-slate-50 dark:bg-slate-800 border border-slate-200 dark:border-slate-700 rounded-2xl pl-10 pr-10 py-3 text-sm focus:outline-none focus:ring-2 focus:ring-brand-200/50 text-slate-700 dark:text-slate-150 font-medium tracking-wide"
                                    >
                                    <button 
                                        type="button" 
                                        onclick="window.togglePasswordVisibilityDirectly()" 
                                        class="absolute right-3.5 text-slate-400 hover:text-slate-600 focus:outline-none p-1 rounded-lg"
                                        title="Tampilkan Sandi"
                                    >
                                        <span id="password-eye-icon-holder">
                                            <i data-lucide="eye" class="w-4.5 h-4.5"></i>
                                        </span>
                                    </button>
                                </div>
                            </div>

                            <button type="submit" class="w-full bg-brand-500 hover:bg-brand-600 text-white rounded-2xl py-3.5 font-bold text-xs tracking-wider uppercase transition-all shadow-lg shadow-brand-100 dark:shadow-none">
                                Verifikasi Kata Sandi
                            </button>
                        </form>

                    </div>
                </div>
            `;
        }
        lucide.createIcons();
    }

    function renderActiveSidebarSection(activeClient, filteredClients, canEdit, isSenior) {
        if (state.sidebarActiveTab === 'clients') {
            return renderClientsManagementList(filteredClients, isSenior);
        } else if (state.sidebarActiveTab === 'settings') {
            return renderSettingsPanel();
        }
        return renderResponsiveWorkspaceHTML(activeClient, filteredClients, canEdit, isSenior);
    }

    function renderResponsiveWorkspaceHTML(activeClient, filteredClients, canEdit, isSenior) {
        if (!activeClient) {
            return `
                <div class="glass-card p-12 rounded-4xl text-center flex flex-col items-center justify-center h-[450px]">
                    <i data-lucide="smile" class="w-16 h-16 text-brand-300 mb-4 animate-bounce"></i>
                    <h3 class="text-lg font-bold text-slate-800 dark:text-white">Pilih Klien untuk Memulai</h3>
                    <p class="text-sm text-slate-400 dark:text-slate-400 max-w-sm mt-1">Gunakan panel navigasi kiri untuk memuat semua kebutuhan instruksi guideline multimedia.</p>
                </div>
            `;
        }

        const isCarouselTab = (state.activeTab === 'carousel');
        const isShortTab = (state.activeTab === 'short');
        const isLongTab = (state.activeTab === 'long');

        return `
            <div class="flex flex-col gap-5 md:gap-6 max-w-7xl mx-auto w-full font-sans">
                
                <!-- Active Client Banner -->
                <div class="relative overflow-hidden rounded-3xl glass-card p-5 md:p-6 flex flex-col md:flex-row md:items-center justify-between gap-5 shadow-sm border border-brand-200 dark:border-slate-800">
                    <div class="absolute -right-12 -bottom-12 w-48 h-48 bg-gradient-to-tr from-brand-100/30 to-brand-300/10 rounded-full blur-2xl pointer-events-none"></div>
                    
                    <div class="flex items-center gap-4 md:gap-5 z-10">
                        <!-- Uploadable Client Profile Logo Photo -->
                        <div class="relative w-14 h-14 md:w-20 md:h-20 group shrink-0">
                            <img src="${activeClient.logo}" onerror="this.src='https://placehold.co/150x150/bae2fd/0e93eb?text=${encodeURIComponent(activeClient.name[0])}'" class="w-full h-full rounded-2xl md:rounded-3xl object-cover border-2 border-white dark:border-slate-800 shadow-lg" alt="">
                            ${canEdit ? `
                                <label class="absolute inset-0 bg-black/50 rounded-2xl md:rounded-3xl flex items-center justify-center opacity-0 group-hover:opacity-100 transition-opacity cursor-pointer" title="Ubah Foto Klien">
                                    <input type="file" accept="image/png,image/jpeg" class="hidden" onchange="handleClientLogoUpload(event, '${activeClient.id}')">
                                    <i data-lucide="camera" class="w-5 h-5 text-white"></i>
                                </label>
                            ` : ''}
                        </div>

                        <div>
                            <div class="flex items-center gap-2">
                                <span class="px-2 py-0.5 bg-brand-50 dark:bg-slate-800 border border-brand-100/50 dark:border-slate-700/50 text-brand-600 dark:text-brand-300 font-bold text-[9px] rounded-full uppercase tracking-wider">Klien Aktif</span>
                            </div>
                            
                            <!-- Inline Edit Client Name for Senior Editor -->
                            ${canEdit ? `
                                <div class="flex items-center gap-2 mt-1">
                                    <input type="text" value="${activeClient.name}" onchange="window.updateClientName('${activeClient.id}', this.value)" class="bg-transparent border-b border-dashed border-slate-300 dark:border-slate-700 focus:border-brand-500 focus:outline-none font-bold text-base md:text-xl text-slate-800 dark:text-white tracking-tight py-0.5 max-w-[200px] sm:max-w-[300px] md:max-w-[400px]" title="Klik untuk mengedit nama klien">
                                    <i data-lucide="edit-2" class="w-3.5 h-3.5 text-slate-400"></i>
                                </div>
                            ` : `
                                <h2 class="font-bold text-base md:text-xl text-slate-800 dark:text-white tracking-tight mt-1 leading-tight">${activeClient.name}</h2>
                            `}
                            
                            <div class="mt-1.5 flex items-center gap-2">
                                <span class="text-xs text-slate-400 font-semibold">Editor:</span>
                                ${canEdit ? `
                                    <select onchange="updateClientField('assignedEditor', this.value)" class="bg-white dark:bg-slate-850 border border-slate-200 dark:border-slate-700 rounded-xl text-xs font-bold text-brand-700 dark:text-brand-300 px-3 py-1 focus:ring-2 focus:ring-brand-200">
                                        <option value="Dina" ${activeClient.assignedEditor === 'Dina' ? 'selected' : ''}>Dina</option>
                                        <option value="Nopi" ${activeClient.assignedEditor === 'Nopi' ? 'selected' : ''}>Nopi</option>
                                        <option value="Diva" ${activeClient.assignedEditor === 'Diva' ? 'selected' : ''}>Diva</option>
                                    </select>
                                ` : `
                                    <span class="bg-brand-50 dark:bg-slate-800 border border-brand-100/80 dark:border-slate-700/80 px-2.5 py-0.5 rounded-lg text-xs font-bold text-brand-700 dark:text-brand-300">
                                        ${activeClient.assignedEditor || 'Dina'}
                                    </span>
                                `}
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Sub Format Tabs (Short, Long, Carousel) -->
                <div class="flex bg-slate-100 dark:bg-slate-850 p-1 rounded-2xl gap-1">
                    <button onclick="setFormatTab('short')" class="flex-1 py-2 text-xs font-bold rounded-xl transition-all flex items-center justify-center gap-1.5 ${state.activeTab === 'short' ? 'bg-white dark:bg-slate-800 text-brand-600 dark:text-white shadow-sm' : 'text-slate-500 hover:text-slate-700'}" title="Konten Rasio 9:16">
                        <i data-lucide="smartphone" class="w-4 h-4"></i>
                        Shorts (9:16)
                    </button>
                    <button onclick="setFormatTab('long')" class="flex-1 py-2 text-xs font-bold rounded-xl transition-all flex items-center justify-center gap-1.5 ${state.activeTab === 'long' ? 'bg-white dark:bg-slate-800 text-brand-600 dark:text-white shadow-sm' : 'text-slate-500 hover:text-slate-700'}" title="Konten Rasio Panjang 9:16">
                        <i data-lucide="video" class="w-4 h-4"></i>
                        Long (9:16)
                    </button>
                    <button onclick="setFormatTab('carousel')" class="flex-1 py-2 text-xs font-bold rounded-xl transition-all flex items-center justify-center gap-1.5 ${state.activeTab === 'carousel' ? 'bg-white dark:bg-slate-800 text-brand-600 dark:text-white shadow-sm' : 'text-slate-500 hover:text-slate-700'}">
                        <i data-lucide="layers" class="w-4 h-4"></i>
                        Carousel (4:5)
                    </button>
                </div>

                <!-- CORE WORKSPACE PANEL -->
                <div class="flex flex-col gap-6">
                    
                    <!-- 1. Guideline Slide (16:9 Aspect Ratio) - Now GLOBAL per Client (Revisions 1, 2, 5) -->
                    ${renderGuidelineSlideSection(activeClient, canEdit)}

                    <!-- 2. Global Client Asset Modules (Color Palette, Graphic Elements, and Typeface) -->
                    <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
                        
                        <!-- Global Color Palette -->
                        <div class="glass-card p-5 rounded-3xl flex flex-col justify-between gap-4 border border-brand-100/50">
                            <div>
                                <h4 class="font-bold text-slate-800 dark:text-white text-xs flex items-center gap-2 mb-1">
                                    <i data-lucide="palette" class="w-4.5 h-4.5 text-brand-500"></i>
                                    Color Palette
                                </h4>
                                <p class="text-[10px] text-slate-400 mb-3">Klik kode warna untuk menyalin instan.</p>
                            </div>

                            <div class="flex flex-wrap gap-2 max-h-[160px] overflow-y-auto">
                                ${!(activeClient.colorPalette && activeClient.colorPalette.length) ? `
                                    <p class="text-xs text-slate-400 italic py-2">Belum ada warna disisipkan.</p>
                                ` : activeClient.colorPalette.map(item => `
                                    <div onclick="copyColorToClipboard('${item.hex}')" class="group relative cursor-pointer flex items-center gap-2 bg-white dark:bg-slate-900 border border-slate-100 dark:border-slate-800 p-1.5 pr-3 rounded-xl shadow-sm transition-all select-none">
                                        <div class="w-6 h-6 rounded-lg border shadow-inner shrink-0" style="background-color: ${item.hex};"></div>
                                        <div class="text-left">
                                            <p class="text-[10px] font-bold text-slate-700 dark:text-slate-200 truncate leading-tight">${item.name}</p>
                                            <p class="text-[9px] text-slate-400 font-mono tracking-wider">${item.hex}</p>
                                        </div>
                                        ${canEdit ? `
                                            <button onclick="event.stopPropagation(); deleteAssetItem('colorPalette', '${item.id}')" class="ml-1 text-rose-400 hover:text-rose-600 transition-colors z-10">
                                                <i data-lucide="x" class="w-3 h-3"></i>
                                            </button>
                                        ` : ''}
                                    </div>
                                `).join('')}
                            </div>

                            ${canEdit ? `
                                <form onsubmit="addColorPaletteItem(event)" class="mt-2 border-t border-slate-100 dark:border-slate-800 pt-3 flex flex-col gap-1.5">
                                    <input type="text" id="new-color-name" placeholder="Nama warna..." class="w-full bg-white dark:bg-slate-800 border border-slate-200 dark:border-slate-700 rounded-xl px-3 py-1.5 text-xs focus:outline-none">
                                    <div class="flex gap-1.5">
                                        <input type="text" id="new-color-hex" required placeholder="Hex Code (Cth: #FF3E6C)" class="flex-1 bg-white dark:bg-slate-800 border border-slate-200 dark:border-slate-700 rounded-xl px-3 py-1.5 text-xs focus:outline-none">
                                        <button type="submit" class="bg-brand-500 hover:bg-brand-600 text-white font-bold text-[10px] px-3 py-1.5 rounded-xl transition-all">
                                            Tambah
                                        </button>
                                    </div>
                                </form>
                            ` : ''}
                        </div>

                        <!-- Global Graphic Elements - Masonry Dynamic Layout (Revision 3) -->
                        <div class="glass-card p-5 rounded-3xl flex flex-col justify-between gap-4 border border-brand-100/50">
                            <div>
                                <h4 class="font-bold text-slate-800 dark:text-white text-xs flex items-center gap-2 mb-1">
                                    <i data-lucide="image" class="w-4.5 h-4.5 text-brand-500"></i>
                                    Graphic Element
                                </h4>
                                <p class="text-[10px] text-slate-400 mb-3">Asset stiker atau overlay khusus klien.</p>
                            </div>

                            <!-- Masonry layout using CSS columns adapts beautifully to native height -->
                            <div class="columns-2 gap-2 max-h-[160px] overflow-y-auto pr-1">
                                ${!(activeClient.graphicElements && activeClient.graphicElements.length) ? `
                                    <div class="col-span-2 text-xs text-slate-400 italic py-2 text-center">Belum ada asset diunggah.</div>
                                ` : activeClient.graphicElements.map(item => `
                                    <div class="break-inside-avoid bg-white dark:bg-slate-900 border border-slate-100 dark:border-slate-800 rounded-xl p-1.5 flex flex-col gap-1.5 relative group mb-2 shadow-sm">
                                        <img class="w-full h-auto object-contain rounded-lg" src="${item.url}" alt="">
                                        <div class="text-left px-1">
                                            <p class="text-[9px] font-extrabold text-slate-800 dark:text-slate-200 truncate" title="${item.title}">${item.title}</p>
                                            <p class="text-[8px] text-slate-400 truncate mt-0.5" title="${item.description || ''}">${item.description || ''}</p>
                                        </div>
                                        <div class="absolute top-1 right-1 flex gap-1 opacity-0 group-hover:opacity-100 transition-opacity">
                                            <button onclick="window.forceDownload('${item.url}', '${item.name}')" class="p-1 bg-white/90 rounded-lg text-brand-600 shadow" title="Download">
                                                <i data-lucide="download" class="w-3 h-3"></i>
                                            </button>
                                            ${canEdit ? `
                                                <button onclick="deleteAssetItem('graphicElements', '${item.id}')" class="p-1 bg-white/90 rounded-lg text-rose-500 shadow" title="Hapus">
                                                    <i data-lucide="trash-2" class="w-3 h-3"></i>
                                                </button>
                                            ` : ''}
                                        </div>
                                    </div>
                                `).join('')}
                            </div>

                            ${canEdit ? `
                                <div class="mt-2 border-t border-slate-100 dark:border-slate-800 pt-3 flex flex-col gap-1.5">
                                    <input type="text" id="upload-title-graphicElements" placeholder="Judul Element..." class="w-full bg-white dark:bg-slate-800 border border-slate-200 dark:border-slate-700 rounded-xl px-2.5 py-1 text-xs focus:outline-none">
                                    <input type="text" id="upload-desc-graphicElements" placeholder="Keterangan..." class="w-full bg-white dark:bg-slate-800 border border-slate-200 dark:border-slate-700 rounded-xl px-2.5 py-1 text-xs focus:outline-none">
                                    <label class="block w-full border border-dashed border-brand-300 hover:border-brand-500 rounded-xl p-2 text-center cursor-pointer bg-brand-50/20 hover:bg-brand-50/50 transition-all">
                                        <input type="file" accept="image/png,image/jpeg" class="hidden" onchange="handleAssetUpload(event, 'graphicElements')">
                                        <span class="text-[10px] font-bold text-brand-600 flex items-center justify-center gap-1.5">
                                            <i data-lucide="upload-cloud" class="w-4 h-4"></i>
                                            Pilih File Gambar
                                        </span>
                                    </label>
                                    <span id="graphicElements-upload-feedback" class="text-[9px] text-slate-400 block"></span>
                                </div>
                            ` : ''}
                        </div>

                        <!-- Global Typeface -->
                        <div class="glass-card p-5 rounded-3xl flex flex-col justify-between gap-4 border border-brand-100/50">
                            <div>
                                <h4 class="font-bold text-slate-800 dark:text-white text-xs flex items-center gap-2 mb-1">
                                    <i data-lucide="type" class="w-4.5 h-4.5 text-brand-500"></i>
                                    Typeface
                                </h4>
                                <p class="text-[10px] text-slate-400 mb-3">Unduh berkas typeface khusus brand klien.</p>
                            </div>

                            <div class="flex flex-col gap-2 max-h-[160px] overflow-y-auto pr-1">
                                ${!(activeClient.fonts && activeClient.fonts.length) ? `
                                    <p class="text-xs text-slate-400 italic py-2 text-center">Belum ada berkas typeface.</p>
                                ` : activeClient.fonts.map(item => `
                                    <div class="bg-white dark:bg-slate-900 border border-slate-100 dark:border-slate-800 rounded-xl p-2 flex items-center justify-between shadow-sm">
                                        <div class="flex items-center gap-2 overflow-hidden">
                                            <i data-lucide="folder-archive" class="w-6 h-6 text-brand-400 shrink-0"></i>
                                            <div class="text-left overflow-hidden">
                                                <p class="text-[10px] font-bold text-slate-700 dark:text-slate-200 truncate" title="${item.name}">${item.name}</p>
                                            </div>
                                        </div>
                                        <div class="flex items-center gap-1">
                                            <button onclick="window.forceDownload('${item.url}', '${item.name}')" class="text-brand-500 p-1.5 rounded-lg hover:bg-brand-50" title="Unduh Typeface">
                                                <i data-lucide="download" class="w-4 h-4"></i>
                                            </button>
                                            ${canEdit ? `
                                                <button onclick="deleteAssetItem('fonts', '${item.id}')" class="text-rose-400 p-1.5 rounded-lg hover:bg-rose-50" title="Hapus">
                                                    <i data-lucide="trash-2" class="w-4 h-4"></i>
                                                </button>
                                            ` : ''}
                                        </div>
                                    </div>
                                `).join('')}
                            </div>

                            ${canEdit ? `
                                <div class="mt-2">
                                    <label class="block w-full border border-dashed border-brand-300 hover:border-brand-500 rounded-xl p-2.5 text-center cursor-pointer bg-brand-50/20 hover:bg-brand-50/50 transition-all">
                                        <input type="file" accept=".zip,.ttf,.otf" class="hidden" onchange="handleAssetUpload(event, 'fonts')">
                                        <span class="text-[10px] font-bold text-brand-600 flex items-center justify-center gap-1.5">
                                            <i data-lucide="upload-cloud" class="w-4 h-4"></i>
                                            Unggah Berkas Baru
                                        </span>
                                    </label>
                                    <span id="fonts-upload-feedback" class="text-[9px] text-slate-400 block"></span>
                                </div>
                            ` : ''}
                        </div>

                    </div>

                    <!-- 3. Format Specific Output Sections -->
                    ${renderContohOutputSection(activeClient, state.activeTab, activeClient[state.activeTab] || createEmptyTab(state.activeTab), canEdit)}

                    <!-- 4. SFX and Transitions (Rendered only on Long Tab content formats) -->
                    ${isLongTab ? `
                        <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                            
                            <!-- Transitions Section with Square 1:1 format -->
                            <div class="glass-card p-5 rounded-3xl flex flex-col justify-between gap-4 border border-brand-100/50">
                                <div>
                                    <h4 class="font-bold text-slate-800 dark:text-white text-xs flex items-center gap-2 mb-1">
                                        <i data-lucide="move-right" class="w-4.5 h-4.5 text-brand-500"></i>
                                        Transisi
                                    </h4>
                                    <p class="text-[10px] text-slate-400 mb-3">Foto transisi layout 1:1 lengkap dengan keterangan.</p>
                                </div>

                                <div class="grid grid-cols-2 gap-3 max-h-[220px] overflow-y-auto pr-1">
                                    ${!(activeClient[state.activeTab].transitions && activeClient[state.activeTab].transitions.length) ? `
                                        <div class="col-span-2 text-xs text-slate-400 italic py-4 text-center">Belum ada transisi ditambahkan.</div>
                                    ` : activeClient[state.activeTab].transitions.map(item => `
                                        <div class="bg-white dark:bg-slate-900 border border-slate-100 dark:border-slate-800 rounded-2xl p-2 flex flex-col gap-2 items-center text-center shadow-sm relative group">
                                            <div class="aspect-square w-16 h-16 bg-slate-50 dark:bg-slate-850 rounded-xl overflow-hidden shrink-0 border dark:border-slate-800">
                                                <img class="w-full h-full object-cover" src="${item.url}" alt="">
                                            </div>
                                            <div class="flex-1 overflow-hidden min-w-0">
                                                <p class="text-xs font-bold text-slate-800 dark:text-slate-200 truncate leading-tight">${item.title}</p>
                                                <p class="text-[10px] text-slate-400 mt-1 line-clamp-2">${item.description || 'Tanpa keterangan.'}</p>
                                            </div>

                                            <div class="absolute top-1 right-1 flex gap-1 opacity-0 group-hover:opacity-100 transition-opacity">
                                                <button onclick="window.forceDownload('${item.url}', '${item.name}')" class="p-1 bg-white/90 rounded-lg text-brand-600 shadow" title="Download">
                                                    <i data-lucide="download" class="w-3 h-3"></i>
                                                </button>
                                                ${canEdit ? `
                                                    <button onclick="deleteAssetItem('transitions', '${item.id}')" class="p-1 bg-white/90 rounded-lg text-rose-500 shadow" title="Hapus">
                                                        <i data-lucide="trash-2" class="w-3 h-3"></i>
                                                    </button>
                                                ` : ''}
                                            </div>
                                        </div>
                                    `).join('')}
                                </div>

                                ${canEdit ? `
                                    <div class="mt-2 border-t border-slate-100 dark:border-slate-800 pt-3 flex flex-col gap-1.5">
                                        <input type="text" id="upload-title-transitions" placeholder="Judul Transisi..." class="w-full bg-white dark:bg-slate-800 border border-slate-200 dark:border-slate-700 rounded-xl px-2.5 py-1.5 text-xs focus:outline-none">
                                        <input type="text" id="upload-desc-transitions" placeholder="Keterangan transisi..." class="w-full bg-white dark:bg-slate-800 border border-slate-200 dark:border-slate-700 rounded-xl px-2.5 py-1.5 text-xs focus:outline-none">
                                        
                                        <label class="block w-full border border-dashed border-brand-300 hover:border-brand-500 rounded-xl p-2 text-center cursor-pointer bg-brand-50/20 hover:bg-brand-50/50 transition-all">
                                            <input type="file" accept="image/png,image/jpeg" class="hidden" onchange="handleAssetUpload(event, 'transitions')">
                                            <span class="text-[10px] font-bold text-brand-600 flex items-center justify-center gap-1.5">
                                                <i data-lucide="upload-cloud" class="w-4 h-4"></i>
                                                Pilih Foto Transisi
                                            </span>
                                        </label>
                                        <span id="transitions-upload-feedback" class="text-[9px] text-slate-400 block"></span>
                                    </div>
                                ` : ''}
                            </div>

                            <!-- SFX Collection Board -->
                            <div class="glass-card p-5 rounded-3xl flex flex-col justify-between gap-4 border border-brand-100/50">
                                <div>
                                    <h4 class="font-bold text-slate-800 dark:text-white text-xs flex items-center gap-2 mb-1">
                                        <i data-lucide="music" class="w-4.5 h-4.5 text-brand-500"></i>
                                        Koleksi SFX
                                    </h4>
                                    <p class="text-[10px] text-slate-400 mb-3">Klik tombol play untuk memutar audio, atau tombol unduh.</p>
                                </div>

                                <div class="flex flex-col gap-2 max-h-[180px] overflow-y-auto pr-1">
                                    ${!(activeClient[state.activeTab].sfx && activeClient[state.activeTab].sfx.length) ? `
                                        <p class="text-xs text-slate-400 italic py-3 text-center">Belum ada SFX ditambahkan.</p>
                                    ` : activeClient[state.activeTab].sfx.map(item => `
                                        <div class="bg-white dark:bg-slate-900 border border-slate-100 dark:border-slate-800 rounded-2xl p-2 flex items-center justify-between shadow-sm">
                                            <div class="flex items-center gap-2 overflow-hidden">
                                                <button onclick="window.playSynthesizedSFX('${item.type}')" class="w-8 h-8 bg-brand-50 dark:bg-slate-800 hover:bg-brand-100 dark:hover:bg-slate-700 rounded-xl text-brand-500 flex items-center justify-center shrink-0">
                                                    <i data-lucide="play" class="w-4 h-4"></i>
                                                </button>
                                                <span class="text-xs font-bold text-slate-700 dark:text-slate-200 truncate" title="${item.name}">${item.name}</span>
                                            </div>
                                            <div class="flex items-center gap-1">
                                                <button onclick="window.forceDownload('${item.url || ''}', '${item.name}')" class="text-brand-500 hover:text-brand-600 p-1.5 rounded-lg hover:bg-brand-50 shrink-0" title="Unduh SFX">
                                                    <i data-lucide="download" class="w-4 h-4"></i>
                                                </button>
                                                ${canEdit ? `
                                                    <button onclick="deleteAssetItem('sfx', '${item.id}')" class="text-rose-400 hover:text-rose-600 p-1.5 rounded-lg shrink-0" title="Hapus">
                                                        <i data-lucide="trash-2" class="w-4 h-4"></i>
                                                    </button>
                                                ` : ''}
                                            </div>
                                        </div>
                                    `).join('')}
                                </div>

                                ${canEdit ? `
                                    <div>
                                        <label class="block w-full border border-dashed border-brand-300 hover:border-brand-500 rounded-xl p-2.5 text-center cursor-pointer bg-brand-50/20 hover:bg-brand-50/50 transition-all">
                                            <input type="file" accept=".mp3,.wav" class="hidden" onchange="handleAssetUpload(event, 'sfx')">
                                            <span class="text-[10px] font-bold text-brand-600 flex items-center justify-center gap-1.5">
                                                <i data-lucide="upload-cloud" class="w-4 h-4"></i>
                                                Pilih Audio SFX
                                            </span>
                                        </label>
                                        <span id="sfx-upload-feedback" class="text-[9px] text-slate-400 block"></span>
                                    </div>
                                ` : ''}
                            </div>

                        </div>
                    ` : ''}

                    <!-- 5. Tautan Referensi Tambahan -->
                    <div class="glass-card p-5 rounded-3xl flex flex-col gap-4 border border-brand-100/50 font-sans">
                        <h4 class="font-bold text-slate-800 dark:text-white text-xs flex items-center gap-2">
                            <i data-lucide="link" class="w-4.5 h-4.5 text-brand-500"></i>
                            Tautan Referensi Konten
                        </h4>

                        <div class="flex flex-col gap-2 max-h-[160px] overflow-y-auto pr-1">
                            ${!(activeClient[state.activeTab].links && activeClient[state.activeTab].links.length) ? `
                                <p class="text-xs text-slate-400 italic text-center py-2">Belum ada tautan referensi.</p>
                            ` : activeClient[state.activeTab].links.map(item => `
                                <div class="bg-white dark:bg-slate-900 border border-slate-100 dark:border-slate-800 rounded-2xl p-2.5 flex items-center justify-between shadow-sm">
                                    <div class="flex items-center gap-2 overflow-hidden">
                                        ${getSocialIcon(item.url)}
                                        <p class="text-xs font-bold text-slate-700 dark:text-slate-200 truncate" title="${item.title}">${item.title}</p>
                                    </div>
                                    <div class="flex items-center gap-1">
                                        <a href="${item.url}" target="_blank" class="bg-brand-50 dark:bg-slate-800 text-brand-600 dark:text-brand-300 hover:bg-brand-100 dark:hover:bg-slate-700 font-bold text-xs px-3 py-1.5 rounded-xl transition-all">
                                            Buka Link
                                        </a>
                                        ${canEdit ? `
                                            <button onclick="deleteAssetItem('links', '${item.id}')" class="text-rose-400 p-1.5 rounded-lg">
                                                <i data-lucide="trash-2" class="w-4 h-4"></i>
                                            </button>
                                        ` : ''}
                                    </div>
                                </div>
                            `).join('')}
                        </div>

                        ${canEdit ? `
                            <form onsubmit="addCustomLink(event)" class="border-t border-slate-100 dark:border-slate-800 pt-3 flex flex-col gap-2">
                                <p class="text-[10px] font-extrabold text-slate-500 uppercase tracking-wider">Tambah Tautan Referensi</p>
                                <div class="flex gap-2">
                                    <input type="text" id="new-link-title" required placeholder="Judul Tautan (Cth: Inspirasi TikTok)" class="flex-1 bg-white dark:bg-slate-800 border border-slate-200 dark:border-slate-700 rounded-xl p-2.5 text-xs focus:outline-none focus:ring-2 focus:ring-brand-200 transition-all">
                                    <input type="url" id="new-link-url" required placeholder="https://..." class="flex-1 bg-white dark:bg-slate-800 border border-slate-200 dark:border-slate-700 rounded-xl p-2.5 text-xs focus:outline-none focus:ring-2 focus:ring-brand-200 transition-all">
                                </div>
                                <button type="submit" class="w-full bg-slate-800 hover:bg-slate-900 text-white rounded-xl py-2 font-bold text-xs transition-all flex items-center justify-center gap-1">
                                    <i data-lucide="plus" class="w-3.5 h-3.5"></i>
                                    Tambahkan Link
                                </button>
                            </form>
                        ` : ''}
                    </div>

                    <!-- 6. Project Instruction Details -->
                    <div class="glass-card p-5 md:p-6 rounded-3xl flex flex-col gap-4 border border-brand-100/50">
                        <div class="flex items-center justify-between">
                            <h3 class="font-bold text-xs text-slate-800 dark:text-white flex items-center gap-2">
                                <i data-lucide="align-left" class="w-5 h-5 text-brand-500"></i>
                                Keterangan Detail Guideline Project (${state.activeTab.toUpperCase()})
                            </h3>
                        </div>
                        
                        ${canEdit ? `
                            <textarea 
                                onchange="updateClientField('description', this.value)"
                                rows="4"
                                placeholder="Masukkan detail instruksi pacing, gaya visual, atau transisi khusus format ini..."
                                class="w-full bg-white dark:bg-slate-800 border border-slate-200 dark:border-slate-700 rounded-2xl p-4 text-sm focus:outline-none focus:ring-2 focus:ring-brand-200 transition-all"
                            >${activeClient[state.activeTab].description || ''}</textarea>
                        ` : `
                            <div class="bg-white/80 dark:bg-slate-900 border border-slate-100 dark:border-slate-800 rounded-2xl p-4 text-sm text-slate-700 dark:text-slate-300 leading-relaxed whitespace-pre-line shadow-inner">
                                ${activeClient[state.activeTab].description || '<em>Belum ada deskripsi instruksi dari Senior Editor untuk format ini.</em>'}
                            </div>
                        `}
                    </div>

                </div>
            </div>
        `;
    }

    function renderGuidelineSlideSection(client, canEdit) {
        const slides = client.guidelineSlides || [];
        const clientIndex = state.activeSlideIndexes[client.id] || 0;
        const currentSlide = slides[clientIndex];

        return `
            <!-- Added premium subtle blue drop shadow & border to ensure popping on pure white images -->
            <div class="glass-card p-5 rounded-3xl flex flex-col gap-4 border border-brand-200 dark:border-slate-800 shadow-[0_20px_50px_rgba(14,147,235,0.12)]">
                <div class="flex items-center justify-between border-b border-brand-100 dark:border-slate-800 pb-3">
                    <div class="flex items-center gap-2">
                        <i data-lucide="presentation" class="w-5 h-5 text-brand-500"></i>
                        <h3 class="font-bold text-slate-800 dark:text-white text-xs">Guideline</h3>
                    </div>
                    <div class="flex items-center gap-2">
                        ${!state.autoplayPaused[client.id] ? `
                            <button onclick="window.manuallyPauseAutoplay('${client.id}')" class="text-[9px] font-bold text-brand-500 hover:text-brand-700 uppercase flex items-center gap-1 px-2 py-0.5 bg-brand-50 rounded-lg" title="Pause Autoplay">
                                <span class="w-1.5 h-1.5 rounded-full bg-green-500 animate-ping"></span>
                                Autoplay On
                            </button>
                        ` : `
                            <span class="text-[9px] font-bold text-slate-400 uppercase px-2 py-0.5 bg-slate-100 rounded-lg">Paused</span>
                        `}
                        <span class="bg-brand-100 dark:bg-slate-800 text-brand-700 dark:text-brand-300 font-bold text-xs px-3 py-1 rounded-full">
                            ${slides.length} Slide Panduan (16:9)
                        </span>
                    </div>
                </div>

                ${slides.length === 0 ? `
                    <div class="bg-white/50 dark:bg-slate-900 border border-dashed border-slate-300 dark:border-slate-700 rounded-3xl p-8 text-center flex flex-col items-center justify-center min-h-[180px]">
                        <i data-lucide="image-off" class="w-10 h-10 text-slate-300 mb-2"></i>
                        <p class="text-sm font-semibold text-slate-400">Belum ada slide guideline.</p>
                    </div>
                ` : `
                    <!-- 16:9 Aspect ratio container with swipe/drag support -->
                    <div class="relative w-full max-w-2xl mx-auto bg-slate-900 rounded-3xl overflow-hidden aspect-[16/9] shadow-inner group select-none cursor-grab active:cursor-grabbing"
                         ontouchstart="window.handleSlideTouchStart(event)"
                         ontouchend="window.handleSlideTouchEnd(event, '${client.id}', ${slides.length})"
                         onmousedown="window.handleSlideMouseDown(event)"
                         onmouseup="window.handleSlideMouseUp(event, '${client.id}', ${slides.length})">
                        <img class="w-full h-full object-cover select-none slide-transition" src="${currentSlide.imageUrl}" alt="Guideline Visual" draggable="false">
                        
                        <div class="absolute top-4 left-4 bg-black/40 backdrop-blur-md text-white text-[11px] font-extrabold px-3.5 py-1.5 rounded-full select-none">
                            Slide ${clientIndex + 1} / ${slides.length}
                        </div>

                        <!-- Manual Navigation triggers - POP UP BLUE BRAND with Beauty Shadow (Revision 1) -->
                        <div class="absolute inset-y-0 inset-x-3 flex items-center justify-between opacity-0 group-hover:opacity-100 transition-opacity">
                            <button onclick="event.stopPropagation(); state.autoplayPaused['${client.id}'] = true; changeSlideIndex('${client.id}', -1, ${slides.length})" class="w-10 h-10 rounded-full bg-brand-500/85 hover:bg-brand-600 text-white shadow-lg shadow-brand-500/30 backdrop-blur-md flex items-center justify-center transition-all">
                                <i data-lucide="chevron-left" class="w-5 h-5"></i>
                            </button>
                            <button onclick="event.stopPropagation(); state.autoplayPaused['${client.id}'] = true; changeSlideIndex('${client.id}', 1, ${slides.length})" class="w-10 h-10 rounded-full bg-brand-500/85 hover:bg-brand-600 text-white shadow-lg shadow-brand-500/30 backdrop-blur-md flex items-center justify-center transition-all">
                                <i data-lucide="chevron-right" class="w-5 h-5"></i>
                            </button>
                        </div>
                    </div>

                    <!-- Shape khusus di bawah gambar presentasi untuk Judul & Keterangan -->
                    <div class="mt-2 bg-brand-50/50 dark:bg-slate-900/60 border border-brand-100/50 dark:border-slate-800/80 p-5 rounded-3xl text-left shadow-inner flex flex-col gap-1.5 relative overflow-hidden">
                        <div class="absolute top-0 right-0 w-24 h-24 bg-brand-300/10 rounded-full blur-xl pointer-events-none"></div>
                        <span class="text-[10px] text-brand-600 dark:text-brand-400 uppercase font-extrabold tracking-widest flex items-center gap-1">
                            <span class="w-1.5 h-1.5 rounded-full bg-brand-500 animate-pulse"></span>
                            Instruksi Panduan Slide ${clientIndex + 1}
                        </span>
                        <p class="text-xs md:text-sm text-slate-700 dark:text-slate-300 font-semibold leading-relaxed">
                            ${currentSlide.text}
                        </p>
                    </div>
                `}

                ${canEdit ? `
                    <div class="border-t border-brand-100 dark:border-slate-800 pt-3 mt-1">
                        <form onsubmit="addGuidelineSlide(event)" class="flex flex-col gap-3">
                            <p class="text-xs font-bold text-slate-500">Tambah Slide Guideline 16:9</p>
                            <div class="grid grid-cols-1 md:grid-cols-2 gap-3">
                                <input type="file" id="new-gslide-image" accept="image/png,image/jpeg" class="w-full bg-white dark:bg-slate-800 border border-slate-200 dark:border-slate-700 rounded-xl p-2 text-xs focus:outline-none">
                                <input type="text" id="new-gslide-text" required placeholder="Teks instruksi slide" class="w-full bg-white dark:bg-slate-800 border border-slate-200 dark:border-slate-700 rounded-xl p-2.5 text-xs focus:outline-none">
                            </div>
                            <div class="flex justify-between items-center">
                                ${slides.length > 0 ? `
                                    <button type="button" onclick="deleteGuidelineSlide('${currentSlide.id}')" class="bg-rose-50 hover:bg-rose-100 text-rose-500 text-xs font-bold px-3 py-2 rounded-xl transition-all flex items-center gap-1">
                                        <i data-lucide="trash-2" class="w-3.5 h-3.5"></i>
                                        Hapus Slide Aktif
                                    </button>
                                ` : '<div></div>'}
                                <button type="submit" class="bg-brand-500 hover:bg-brand-600 text-white font-bold text-xs px-4 py-2.5 rounded-xl transition-all flex items-center gap-1">
                                    <i data-lucide="plus" class="w-3.5 h-3.5"></i>
                                    Simpan Slide
                                </button>
                            </div>
                        </form>
                    </div>
                ` : ''}
            </div>
        `;
    }

    function renderContohOutputSection(client, tabName, tabData, canEdit) {
        const videos = tabData.contohOutput || [];

        if (tabName === 'carousel') {
            return `
                <div class="glass-card p-5 rounded-3xl flex flex-col gap-6 border border-brand-100/50">
                    <div>
                        <h3 class="font-bold text-slate-800 dark:text-white text-xs flex items-center gap-2">
                            <i data-lucide="layers" class="w-5 h-5 text-brand-500"></i>
                            Contoh Output Carousel (Rasio 4:5)
                        </h3>
                        <p class="text-[10px] text-slate-400 mt-0.5">Daftar file gambar acuan berasio tegak 4:5 untuk visual Carousel.</p>
                    </div>

                    <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-6">
                        ${videos.length === 0 ? `
                            <div class="col-span-3 py-12 flex flex-col items-center justify-center bg-slate-50 dark:bg-slate-900 border border-dashed rounded-3xl text-center">
                                <i data-lucide="image" class="w-8 h-8 text-slate-300 mb-1"></i>
                                <p class="text-xs text-slate-400 font-semibold">Belum ada gambar output Carousel.</p>
                            </div>
                        ` : videos.map(item => `
                            <div class="bg-slate-50 dark:bg-slate-900 border border-slate-100 dark:border-slate-800 p-4 rounded-3xl flex flex-col justify-between gap-3 relative group">
                                <div class="relative aspect-[4/5] w-full max-w-[180px] mx-auto bg-slate-100 dark:bg-slate-950 rounded-2xl overflow-hidden shadow-sm border">
                                    <img class="w-full h-full object-cover" src="${item.url}" alt="">
                                </div>
                                <div class="bg-white dark:bg-slate-850 p-3 rounded-2xl border text-left">
                                    <h4 class="text-xs font-bold text-slate-800 dark:text-slate-150 truncate">${item.title}</h4>
                                    <p class="text-[11px] text-slate-500 dark:text-slate-400 mt-1 leading-relaxed">${item.description}</p>
                                </div>
                                ${canEdit ? `
                                    <button onclick="deleteContohOutputVideo('${item.id}')" class="absolute top-6 right-6 p-2 bg-white/95 rounded-xl shadow text-rose-500 hover:bg-rose-50 transition-all">
                                        <i data-lucide="trash-2" class="w-4 h-4"></i>
                                    </button>
                                ` : ''}
                            </div>
                        `).join('')}
                    </div>

                    ${canEdit ? `
                        <div class="border-t border-slate-100 dark:border-slate-800 pt-4">
                            <form onsubmit="addContohOutputVideo(event)" class="flex flex-col gap-3">
                                <p class="text-xs font-bold text-slate-500">Unggah Gambar Carousel Baru (Wajib Rasio 4:5)</p>
                                <div class="grid grid-cols-1 md:grid-cols-3 gap-3">
                                    <div>
                                        <label class="block text-[10px] font-bold text-slate-400 mb-1">File Gambar</label>
                                        <input type="file" id="new-img-file-carousel" required accept="image/png,image/jpeg" class="w-full bg-white dark:bg-slate-800 border border-slate-200 dark:border-slate-700 rounded-xl p-2 text-xs focus:outline-none">
                                    </div>
                                    <div>
                                        <label class="block text-[10px] font-bold text-slate-400 mb-1">Judul Gambar</label>
                                        <input type="text" id="new-img-title-carousel" required placeholder="Slide Cover Utama" class="w-full bg-white dark:bg-slate-800 border border-slate-200 dark:border-slate-700 rounded-xl p-2.5 text-xs focus:outline-none">
                                    </div>
                                    <div>
                                        <label class="block text-[10px] font-bold text-slate-400 mb-1">Keterangan Gambar</label>
                                        <input type="text" id="new-img-desc-carousel" placeholder="Instruksi tipografi slide ini..." class="w-full bg-white dark:bg-slate-800 border border-slate-200 dark:border-slate-700 rounded-xl p-2.5 text-xs focus:outline-none">
                                    </div>
                                </div>
                                <button type="submit" class="bg-brand-500 hover:bg-brand-600 text-white font-bold text-xs px-4 py-2.5 rounded-xl transition-all self-end flex items-center gap-1.5">
                                    <i data-lucide="plus" class="w-4 h-4"></i>
                                    Simpan Carousel
                                </button>
                            </form>
                        </div>
                    ` : ''}
                </div>
            `;
        }

        if (tabName === 'short') {
            return `
                <div class="glass-card p-5 rounded-3xl flex flex-col gap-6 border border-brand-100/50">
                    <div>
                        <h3 class="font-bold text-slate-800 dark:text-white text-xs flex items-center gap-2">
                            <i data-lucide="smartphone" class="w-5 h-5 text-brand-500"></i>
                            Contoh Output Shorts (Rasio 9:16)
                        </h3>
                        <p class="text-[10px] text-slate-400 mt-0.5">Daftar file video acuan berasio vertikal portrait 9:16.</p>
                    </div>

                    <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-6">
                        ${videos.length === 0 ? `
                            <div class="col-span-3 py-12 flex flex-col items-center justify-center bg-slate-50 dark:bg-slate-900 border border-dashed rounded-3xl text-center">
                                <i data-lucide="video" class="w-8 h-8 text-slate-300 mb-1"></i>
                                <p class="text-xs text-slate-400 font-semibold">Belum ada video output Shorts.</p>
                            </div>
                        ` : videos.map(item => `
                            <div class="bg-slate-50 dark:bg-slate-900 border border-slate-100 dark:border-slate-800 p-4 rounded-3xl flex flex-col justify-between gap-3 relative group">
                                <div class="relative aspect-[9/16] w-full max-w-[140px] mx-auto bg-slate-100 dark:bg-slate-950 rounded-2xl overflow-hidden shadow-sm border">
                                    <video class="w-full h-full object-cover" controls src="${item.url}"></video>
                                </div>
                                <div class="bg-white dark:bg-slate-850 p-3 rounded-2xl border text-left">
                                    <h4 class="text-xs font-bold text-slate-800 dark:text-slate-150 truncate">${item.title}</h4>
                                    <p class="text-[11px] text-slate-500 dark:text-slate-400 mt-1 leading-relaxed">${item.description}</p>
                                </div>
                                ${canEdit ? `
                                    <button onclick="deleteContohOutputVideo('${item.id}')" class="absolute top-6 right-6 p-2 bg-white/95 rounded-xl shadow text-rose-500 hover:bg-rose-50 transition-all">
                                        <i data-lucide="trash-2" class="w-4 h-4"></i>
                                    </button>
                                ` : ''}
                            </div>
                        `).join('')}
                    </div>

                    ${canEdit ? `
                        <div class="border-t border-slate-100 dark:border-slate-800 pt-4">
                            <form onsubmit="addContohOutputVideo(event)" class="flex flex-col gap-3">
                                <p class="text-xs font-bold text-slate-500">Unggah Video Shorts Baru (Wajib Rasio 9:16)</p>
                                <div class="grid grid-cols-1 md:grid-cols-3 gap-3">
                                    <div>
                                        <label class="block text-[10px] font-bold text-slate-400 mb-1">File Video</label>
                                        <input type="file" id="new-video-file-short" required accept="video/mp4,video/mov" class="w-full bg-white dark:bg-slate-800 border border-slate-200 dark:border-slate-700 rounded-xl p-2 text-xs focus:outline-none">
                                    </div>
                                    <div>
                                        <label class="block text-[10px] font-bold text-slate-400 mb-1">Judul Video</label>
                                        <input type="text" id="new-video-title-short" required placeholder="Contoh Hook Dinamis" class="w-full bg-white dark:bg-slate-800 border border-slate-200 dark:border-slate-700 rounded-xl p-2.5 text-xs focus:outline-none">
                                    </div>
                                    <div>
                                        <label class="block text-[10px] font-bold text-slate-400 mb-1">Keterangan Video</label>
                                        <input type="text" id="new-video-desc-short" placeholder="Instruksi transisi atau audio hook..." class="w-full bg-white dark:bg-slate-800 border border-slate-200 dark:border-slate-700 rounded-xl p-2.5 text-xs focus:outline-none">
                                    </div>
                                </div>
                                <button type="submit" class="bg-brand-500 hover:bg-brand-600 text-white font-bold text-xs px-4 py-2.5 rounded-xl transition-all self-end flex items-center gap-1.5">
                                    <i data-lucide="plus" class="w-4 h-4"></i>
                                    Simpan Shorts Video
                                </button>
                            </form>
                        </div>
                    ` : ''}
                </div>
            `;
        }

        const categories = ['B-roll', 'Typography', 'Animasi'];
        const categoryMeta = {
            'B-roll': { title: 'B-roll', subtitle: 'Pilihan footage pendukung visual' },
            'Typography': { title: 'Typography', subtitle: 'Gaya visual teks dinamis' },
            'Animasi': { title: 'Visual Animasi (opsional)', subtitle: 'hanya digunakan ketika memang butuh visual yg mudah untuk dipahami audience' }
        };

        return `
            <div class="glass-card p-5 rounded-3xl flex flex-col gap-6 border border-brand-100/50">
                <div>
                    <h3 class="font-bold text-slate-800 dark:text-white text-xs flex items-center gap-2">
                        <i data-lucide="video" class="w-5 h-5 text-brand-500"></i>
                        Contoh Output Long Form (9:16)
                    </h3>
                    <p class="text-[10px] text-slate-400 mt-0.5">Kumpulan video contoh output berasio portrait yang dibagi menjadi sub-kategori utama.</p>
                </div>

                <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
                    ${categories.map(cat => {
                        const filteredVideos = videos.filter(v => v.subCategory === cat);
                        const stateKey = `${client.id}-${tabName}-${cat}`;
                        const currentIdx = state.activeVideoIndexes[stateKey] || 0;
                        const videoToShow = filteredVideos[currentIdx];
                        const meta = categoryMeta[cat] || { title: cat, subtitle: '' };

                        return `
                            <div class="bg-slate-50 dark:bg-slate-900 border border-slate-100 dark:border-slate-800 p-4 rounded-3xl flex flex-col justify-between gap-4">
                                <div>
                                    <h4 class="text-xs font-extrabold uppercase text-brand-600 dark:text-brand-400 tracking-wider border-b pb-1.5">${meta.title}</h4>
                                    ${meta.subtitle ? `<p class="text-[10px] text-slate-400 font-semibold mt-1 leading-normal">${meta.subtitle}</p>` : ''}
                                </div>

                                ${filteredVideos.length === 0 ? `
                                    <div class="h-44 flex flex-col items-center justify-center bg-white dark:bg-slate-850 border border-dashed border-slate-200 dark:border-slate-700 rounded-2xl text-center p-4">
                                        <i data-lucide="film" class="w-8 h-8 text-slate-300 mb-1"></i>
                                        <p class="text-[10px] text-slate-400 font-semibold">Belum ada video acuan.</p>
                                    </div>
                                ` : `
                                    <div class="flex flex-col gap-3 mt-2">
                                        <div class="relative aspect-[9/16] max-h-[220px] w-full max-w-[130px] mx-auto bg-slate-950 rounded-2xl overflow-hidden shadow-inner border">
                                            <video class="w-full h-full object-cover" controls src="${videoToShow.url}"></video>
                                        </div>

                                        <div class="bg-white dark:bg-slate-850 p-3 rounded-2xl border text-left">
                                            <p class="text-[10px] font-extrabold text-slate-400 uppercase tracking-widest mb-1">Catatan Senior</p>
                                            <p class="text-xs text-slate-600 dark:text-slate-300 leading-relaxed font-semibold">
                                                ${videoToShow.note}
                                            </p>
                                        </div>

                                        <div class="flex justify-between items-center text-[10px] text-slate-400 font-bold px-1">
                                            <span>Video ${currentIdx + 1} / ${filteredVideos.length}</span>
                                            
                                            <div class="flex gap-1.5">
                                                <button onclick="changeVideoCarouselIndex('${client.id}', '${tabName}', '${cat}', -1, ${filteredVideos.length})" class="w-5 h-5 bg-white dark:bg-slate-800 border rounded flex items-center justify-center text-slate-500">
                                                    <i data-lucide="chevron-left" class="w-3.5 h-3.5"></i>
                                                </button>
                                                <button onclick="changeVideoCarouselIndex('${client.id}', '${tabName}', '${cat}', 1, ${filteredVideos.length})" class="w-5 h-5 bg-white dark:bg-slate-800 border rounded flex items-center justify-center text-slate-500">
                                                    <i data-lucide="chevron-right" class="w-3.5 h-3.5"></i>
                                                </button>
                                                ${canEdit ? `
                                                    <button onclick="deleteContohOutputVideo('${videoToShow.id}')" class="text-rose-400 hover:text-rose-600 ml-1.5" title="Hapus Video Ini">
                                                        <i data-lucide="trash-2" class="w-3.5 h-3.5"></i>
                                                    </button>
                                                ` : ''}
                                            </div>
                                        </div>
                                    </div>
                                `}
                            </div>
                        `;
                    }).join('')}
                </div>

                ${canEdit ? `
                    <div class="border-t border-slate-100 dark:border-slate-800 pt-4">
                        <form onsubmit="addContohOutputVideo(event)" class="flex flex-col gap-3">
                            <p class="text-xs font-bold text-slate-500">Tambah Contoh Output Video Baru (Rasio 9:16)</p>
                            <div class="grid grid-cols-1 md:grid-cols-3 gap-3">
                                <div>
                                    <label class="block text-[10px] font-bold text-slate-400 mb-1">Video File</label>
                                    <input type="file" id="new-video-file" required accept="video/mp4,video/mov" class="w-full bg-white dark:bg-slate-800 border border-slate-200 dark:border-slate-700 rounded-xl p-2 text-xs focus:outline-none">
                                </div>
                                <div>
                                    <label class="block text-[10px] font-bold text-slate-400 mb-1">Sub-kategori Output</label>
                                    <select id="new-video-subcat" class="w-full bg-white dark:bg-slate-800 border border-slate-200 dark:border-slate-700 rounded-xl p-2.5 text-xs font-bold text-slate-700 dark:text-slate-300 focus:outline-none">
                                        <option value="B-roll">B-roll</option>
                                        <option value="Typography">Typography</option>
                                        <option value="Animasi">Animasi (Visual Animasi)</option>
                                    </select>
                                </div>
                                <div>
                                    <label class="block text-[10px] font-bold text-slate-400 mb-1">Catatan Tambahan Video</label>
                                    <input type="text" id="new-video-note" placeholder="Catatan khusus video ini..." class="w-full bg-white dark:bg-slate-800 border border-slate-200 dark:border-slate-700 rounded-xl p-2.5 text-xs focus:outline-none">
                                </div>
                            </div>
                            <button type="submit" class="bg-brand-500 hover:bg-brand-600 text-white font-bold text-xs py-2.5 rounded-xl transition-all self-end flex items-center gap-1.5">
                                <i data-lucide="plus" class="w-4 h-4"></i>
                                Unggah Contoh Output
                            </button>
                        </form>
                    </div>
                ` : ''}
            </div>
        `;
    }

    function renderClientsManagementList(filteredClients, isSenior) {
        return `
            <div class="max-w-4xl mx-auto flex flex-col gap-6 text-left animate-fade-in">
                <div class="flex items-center justify-between">
                    <div>
                        <h2 class="font-extrabold text-2xl text-slate-800 dark:text-white">Daftar Klien Agensi</h2>
                        <p class="text-xs text-slate-400">Kelola dan lihat daftar klien aktif penugasan Anda.</p>
                    </div>
                    ${isSenior ? `
                        <button onclick="toggleNewClientModal(true)" class="bg-brand-500 hover:bg-brand-600 text-white rounded-2xl px-5 py-3 font-bold text-xs transition-all flex items-center gap-2">
                            <i data-lucide="plus" class="w-4 h-4"></i>
                            Tambah Klien Baru
                        </button>
                    ` : ''}
                </div>

                <div class="relative">
                    <input type="text" 
                        placeholder="Cari nama brand..." 
                        value="${state.searchQuery}"
                        oninput="state.searchQuery = this.value; renderApp();"
                        class="w-full bg-white dark:bg-slate-950 border border-slate-200 dark:border-slate-800 rounded-2xl pl-10 pr-4 py-3 text-sm focus:outline-none focus:ring-2 focus:ring-brand-300 dark:focus:ring-brand-900 transition-all"
                    >
                    <i data-lucide="search" class="w-4 h-4 text-slate-400 absolute left-3.5 top-4"></i>
                </div>

                <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                    ${filteredClients.length === 0 ? `
                        <div class="col-span-2 glass-card p-12 text-center rounded-3xl">
                            <i data-lucide="folder-open" class="w-12 h-12 text-slate-300 mx-auto mb-3"></i>
                            <p class="text-sm font-semibold text-slate-500">Tidak ada klien ditemukan</p>
                        </div>
                    ` : filteredClients.map(c => `
                        <div onclick="selectClient('${c.id}')" class="glass-card p-5 rounded-3xl flex items-center justify-between cursor-pointer hover:border-brand-500 hover:shadow-md transition-all duration-300 animate-fade-in">
                            <div class="flex items-center gap-4">
                                <img src="${c.logo}" onerror="this.src='https://placehold.co/100x100/bae2fd/0e93eb?text=${encodeURIComponent(c.name[0])}'" class="w-14 h-14 rounded-2xl object-cover border shadow-sm">
                                <div class="text-left">
                                    <h3 class="font-bold text-slate-800 dark:text-white text-sm">${c.name}</h3>
                                    <p class="text-[11px] text-slate-400 mt-1 flex items-center gap-1">
                                        <i data-lucide="user-check" class="w-3.5 h-3.5 text-brand-500"></i>
                                        Editor: ${c.assignedEditor || 'Dina'}
                                    </p>
                                </div>
                            </div>
                            
                            <div class="flex items-center gap-3">
                                ${isSenior ? `
                                    <button onclick="event.stopPropagation(); window.confirmDeleteClient('${c.id}')" class="p-2.5 bg-rose-50 dark:bg-rose-950/25 text-rose-500 hover:text-rose-600 hover:bg-rose-100 rounded-xl transition-all" title="Hapus Klien">
                                        <i data-lucide="trash-2" class="w-4 h-4"></i>
                                    </button>
                                ` : ''}
                                <i data-lucide="chevron-right" class="w-5 h-5 text-slate-400"></i>
                            </div>
                        </div>
                    `).join('')}
                </div>
            </div>
        `;
    }

    function renderSettingsPanel() {
        return `
            <div class="max-w-4xl mx-auto font-sans animate-fade-in">
                <div class="mb-6 text-left">
                    <h2 class="font-extrabold text-2xl text-slate-800 dark:text-white">Settings</h2>
                    <p class="text-xs text-slate-400 mt-0.5">Manage your account preferences</p>
                </div>

                <div class="glass-card rounded-3xl overflow-hidden shadow-sm border border-slate-200/60 dark:border-slate-800/60 animate-fade-in">
                    
                    <div class="flex border-b border-slate-100 dark:border-slate-800 bg-slate-50/50 dark:bg-slate-900/50 px-6 pt-3 gap-1 overflow-x-auto">
                        <button onclick="setSettingsTab('profile')" class="px-5 py-3 text-xs font-bold border-b-2 transition-all flex items-center gap-1.5 shrink-0 ${state.settingsActiveTab === 'profile' ? 'border-brand-500 text-brand-600 dark:text-brand-300' : 'border-transparent text-slate-500 hover:text-slate-800'}" >
                            <i data-lucide="user" class="w-4 h-4"></i>
                            Profile
                        </button>
                        <button onclick="setSettingsTab('password')" class="px-5 py-3 text-xs font-bold border-b-2 transition-all flex items-center gap-1.5 shrink-0 ${state.settingsActiveTab === 'password' ? 'border-brand-500 text-brand-600 dark:text-brand-300' : 'border-transparent text-slate-500 hover:text-slate-800'}">
                            <i data-lucide="lock" class="w-4 h-4"></i>
                            Password
                        </button>
                        <button onclick="setSettingsTab('notifications')" class="px-5 py-3 text-xs font-bold border-b-2 transition-all flex items-center gap-1.5 shrink-0 ${state.settingsActiveTab === 'notifications' ? 'border-brand-500 text-brand-600 dark:text-brand-300' : 'border-transparent text-slate-500 hover:text-slate-800'}">
                            <i data-lucide="bell" class="w-4 h-4"></i>
                            Notifications
                        </button>
                        <button onclick="setSettingsTab('appearance')" class="px-5 py-3 text-xs font-bold border-b-2 transition-all flex items-center gap-1.5 shrink-0 ${state.settingsActiveTab === 'appearance' ? 'border-brand-500 text-brand-600 dark:text-brand-300' : 'border-transparent text-slate-500 hover:text-slate-800'}">
                            <i data-lucide="palette" class="w-4 h-4"></i>
                            Appearance
                        </button>
                    </div>

                    <div class="p-6 md:p-8">
                        ${renderInnerSettingsContent()}
                    </div>

                </div>
            </div>
        `;
    }

    function renderInnerSettingsContent() {
        if (state.settingsActiveTab === 'password') {
            return `
                <div class="max-w-md text-left flex flex-col gap-4 animate-fade-in">
                    <h4 class="font-extrabold text-sm text-slate-800 dark:text-white">Ubah Kata Sandi</h4>
                    <div>
                        <label class="block text-[11px] font-bold text-slate-400 uppercase tracking-wider mb-1">Kata Sandi Saat Ini</label>
                        <input type="password" id="settings-current-password" placeholder="••••••••" class="w-full bg-slate-50 dark:bg-slate-800 border border-slate-200 dark:border-slate-700 rounded-xl p-3 text-xs focus:outline-none">
                    </div>
                    <div>
                        <label class="block text-[11px] font-bold text-slate-400 uppercase tracking-wider mb-1">Kata Sandi Baru</label>
                        <input type="password" id="settings-new-password" placeholder="••••••••" class="w-full bg-slate-50 dark:bg-slate-800 border border-slate-200 dark:border-slate-700 rounded-xl p-3 text-xs focus:outline-none">
                    </div>
                    <button onclick="handlePasswordChangeSubmit(event)" class="bg-brand-500 hover:bg-brand-600 text-white font-bold rounded-xl px-5 py-2.5 text-xs transition-all self-start">
                        Ubah Password
                    </button>
                </div>
            `;
        } else if (state.settingsActiveTab === 'notifications') {
            return `
                <div class="max-w-md text-left flex flex-col gap-4 animate-fade-in">
                    <h4 class="font-extrabold text-sm text-slate-800 dark:text-white">Notifikasi Workspace</h4>
                    <p class="text-xs text-slate-400">Atur preferensi pengiriman notifikasi pembaruan guideline video dari Senior Editor.</p>
                    <label class="flex items-center gap-3 cursor-pointer">
                        <input type="checkbox" checked class="w-4 h-4 text-brand-500 rounded focus:ring-0">
                        <span class="text-xs font-bold text-slate-700 dark:text-slate-300">Notifikasi Pop-up Toast Instan</span>
                    </label>
                    <label class="flex items-center gap-3 cursor-pointer">
                        <input type="checkbox" checked class="w-4 h-4 text-brand-500 rounded focus:ring-0">
                        <span class="text-xs font-bold text-slate-700 dark:text-slate-300">Pemberitahuan perubahan via Email</span>
                    </label>
                </div>
            `;
        } else if (state.settingsActiveTab === 'appearance') {
            return `
                <div class="max-w-md text-left flex flex-col gap-4 animate-fade-in">
                    <h4 class="font-extrabold text-sm text-slate-800 dark:text-white">Tema & Visual Tampilan</h4>
                    <p class="text-xs text-slate-400">Sesuaikan tema pengerjaan editing sesuai kenyamanan mata Anda.</p>
                    
                    <div class="grid grid-cols-2 gap-3 mt-2">
                        <div onclick="toggleDarkMode(false)" class="border rounded-2xl p-4 cursor-pointer text-center ${!state.darkMode ? 'border-brand-500 bg-brand-50/20 dark:bg-brand-900/10' : 'border-slate-200'}">
                            <i data-lucide="sun" class="w-6 h-6 mx-auto mb-2 text-amber-500"></i>
                            <span class="text-xs font-extrabold text-slate-700 dark:text-slate-300">Light Mode</span>
                        </div>
                        <div onclick="toggleDarkMode(true)" class="border rounded-2xl p-4 cursor-pointer text-center ${state.darkMode ? 'border-brand-500 bg-brand-50/20 dark:bg-brand-900/10' : 'border-slate-200'}">
                            <i data-lucide="moon" class="w-6 h-6 mx-auto mb-2 text-blue-400"></i>
                            <span class="text-xs font-extrabold text-slate-700 dark:text-slate-300">Dark Mode</span>
                        </div>
                    </div>
                </div>
            `;
        }

        return `
            <form onsubmit="saveProfileSettings(event)" class="text-left flex flex-col gap-6 font-sans animate-fade-in">
                <div class="flex items-center gap-4">
                    <div class="w-16 h-16 rounded-2xl bg-brand-500 text-white flex items-center justify-center font-extrabold text-2xl shadow-md">
                        ${state.currentUser.avatar}
                    </div>
                    <div>
                        <h4 class="font-extrabold text-slate-800 dark:text-white text-md">${state.currentUser.role}</h4>
                        <p class="text-xs text-slate-400">@${state.currentUser.username || 'username'}</p>
                    </div>
                </div>

                <div class="max-w-xl flex flex-col gap-4">
                    <div>
                        <label class="block text-[11px] font-bold text-slate-400 uppercase tracking-wider mb-1">Display Name</label>
                        <input type="text" id="settings-display-name" required value="${state.currentUser.name}" class="w-full bg-slate-50 dark:bg-slate-800 border border-slate-200 dark:border-slate-700 rounded-xl p-3.5 text-xs font-bold text-slate-700 dark:text-slate-200 focus:outline-none focus:ring-2 focus:ring-brand-200">
                    </div>

                    <div>
                        <label class="block text-[11px] font-bold text-slate-400 uppercase tracking-wider mb-1">Username</label>
                        <input type="text" id="settings-username" required value="${state.currentUser.username || 'editor'}" class="w-full bg-slate-50 dark:bg-slate-800 border border-slate-200 dark:border-slate-700 rounded-xl p-3.5 text-xs font-bold text-slate-700 dark:text-slate-200 focus:outline-none focus:ring-2 focus:ring-brand-200">
                    </div>

                    <button type="submit" class="bg-brand-500 hover:bg-brand-600 text-white font-extrabold rounded-xl px-6 py-3 text-xs transition-all self-start shadow-md shadow-brand-100">
                        Save Changes
                    </button>
                </div>
            </form>
        `;
    }
</script>

<!-- Global Toast Notification Container -->
<div id="toast" class="fixed top-6 right-6 z-50 flex items-center gap-3 bg-white px-5 py-3.5 rounded-2xl shadow-xl transition-all duration-300 transform -translate-y-20 opacity-0 pointer-events-none">
    <div id="toast-icon"></div>
    <span id="toast-text" class="text-xs font-bold font-sans"></span>
</div>

<!-- Main UI Injection Node -->
<div id="app-root">
    <div class="flex flex-col items-center justify-center min-h-screen bg-slate-50">
        <div class="w-12 h-12 border-4 border-slate-200 border-t-brand-500 rounded-full animate-spin"></div>
        <p class="mt-4 text-slate-400 text-sm font-medium font-sans">Memuat Workspace Agency...</p>
    </div>
</div>

</body>
</html>
