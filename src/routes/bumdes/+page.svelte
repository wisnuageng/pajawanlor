<script lang="ts">
    import { fly } from 'svelte/transition';
</script>

<svelte:head>
    <title>BUMDes - Pajawanlor</title>
</svelte:head>

<!-- Header -->
<header class="bg-surface-dark py-24 border-b border-surface-dark-elevated">
    <div class="max-w-5xl mx-auto px-4 sm:px-6 lg:px-8 text-center" in:fly={{y: 30, duration: 800}}>
        <div class="inline-flex items-center gap-2 px-4 py-1.5 rounded-pill bg-primary/20 text-primary border border-primary/30 text-sm font-medium mb-6">
            Badan Usaha Milik Desa
        </div>
        <h1 class="text-5xl md:text-6xl font-display text-on-dark tracking-tight mb-6">BUMDes Maju Bersama</h1>
        <p class="text-lg text-on-dark-soft max-w-2xl mx-auto leading-relaxed">
            Pusat pengembangan ekonomi lokal, unit usaha produktif, dan etalase produk unggulan warga Desa Pajawanlor.
        </p>
    </div>
</header>

<main class="bg-canvas py-section">
    <div class="max-w-5xl mx-auto px-4 sm:px-6 lg:px-8 space-y-24">
        
        <!-- Intro & Visi Misi -->
        <section class="grid grid-cols-1 md:grid-cols-2 gap-12 items-center" in:fly={{y: 20, duration: 800, delay: 100}}>
            <div class="space-y-6">
                <h2 class="text-3xl font-display text-ink">Menggerakkan Roda Ekonomi Desa</h2>
                <p class="text-body text-lg leading-relaxed">
                    BUMDes hadir sebagai instrumen kemandirian desa yang bertujuan untuk memaksimalkan potensi ekonomi lokal, membuka lapangan pekerjaan baru, dan mendistribusikan manfaat secara adil bagi seluruh warga Desa Pajawanlor.
                </p>
                <ul class="space-y-4 pt-4">
                    <li class="flex items-start gap-3">
                        <svg class="w-6 h-6 text-primary shrink-0" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" />
                        </svg>
                        <span class="text-body font-medium">Pemberdayaan UMKM lokal</span>
                    </li>
                    <li class="flex items-start gap-3">
                        <svg class="w-6 h-6 text-primary shrink-0" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" />
                        </svg>
                        <span class="text-body font-medium">Pengelolaan sumber daya alam dan pertanian</span>
                    </li>
                    <li class="flex items-start gap-3">
                        <svg class="w-6 h-6 text-primary shrink-0" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" />
                        </svg>
                        <span class="text-body font-medium">Layanan jasa administrasi dan pembayaran</span>
                    </li>
                </ul>
            </div>
            <div class="bg-surface-card rounded-xl border border-hairline p-8 md:p-12 shadow-sm text-center">
                <div class="inline-flex items-center justify-center w-20 h-20 rounded-full bg-surface-soft border border-hairline mb-6 shadow-inner">
                    <svg class="w-10 h-10 text-primary" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" d="M21 13.255A23.931 23.931 0 0112 15c-3.183 0-6.22-.62-9-1.745M16 6V4a2 2 0 00-2-2h-4a2 2 0 00-2 2v2m4 6h.01M5 20h14a2 2 0 002-2V8a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z" />
                    </svg>
                </div>
                <h3 class="text-2xl font-display text-ink mb-4">Mari Bermitra!</h3>
                <p class="text-body mb-8">
                    Kami membuka peluang kerja sama yang saling menguntungkan bagi pelaku usaha, investor, maupun institusi terkait.
                </p>
                <button class="w-full inline-flex justify-center items-center px-6 py-3 rounded-md bg-primary text-on-primary font-medium hover:bg-primary-active transition-colors">
                    Hubungi Pengurus BUMDes
                </button>
            </div>
        </section>

        <!-- Galeri Unit Usaha -->
        <section in:fly={{y: 20, duration: 800, delay: 200}}>
            <h2 class="text-3xl font-display text-ink mb-8 text-center">Galeri & Program BUMDes</h2>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                
                <div class="bg-surface-card rounded-xl overflow-hidden border border-hairline group cursor-pointer shadow-sm hover:shadow-md transition-shadow">
                    <div class="aspect-[4/3] overflow-hidden bg-surface-soft relative">
                        <img 
                            src="/assets/IMG_0601.HEIC" 
                            alt="Pemberdayaan potensi ekonomi Desa" 
                            class="w-full h-full object-cover transition-transform duration-700 group-hover:scale-105"
                            onerror={(e) => { e.currentTarget.src='https://images.unsplash.com/photo-1542838132-92c53300491e?w=800&q=80'; e.currentTarget.onerror=null; }}
                        />
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-medium text-ink mb-2">Pemberdayaan Potensi Ekonomi Desa</h3>
                        <p class="text-body text-sm leading-relaxed">
                            Program inisiatif untuk menggali dan mengoptimalkan potensi ekonomi lokal, mendukung UMKM, serta menciptakan peluang usaha baru bagi kesejahteraan warga desa.
                        </p>
                    </div>
                </div>

                <div class="bg-surface-card rounded-xl overflow-hidden border border-hairline group cursor-pointer shadow-sm hover:shadow-md transition-shadow">
                    <div class="aspect-[4/3] overflow-hidden bg-surface-soft relative">
                        <img 
                            src="/assets/WhatsApp%20Image%202026-09-25%20at%2014.13.42.jpeg" 
                            alt="Pengendalian Sampah" 
                            class="w-full h-full object-cover transition-transform duration-700 group-hover:scale-105"
                            onerror={(e) => { e.currentTarget.src='https://images.unsplash.com/photo-1542838132-92c53300491e?w=800&q=80'; e.currentTarget.onerror=null; }}
                        />
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-medium text-ink mb-2">Pengendalian Sampah</h3>
                        <p class="text-body text-sm leading-relaxed">
                            Fokus pada pelestarian lingkungan melalui pengelolaan dan daur ulang sampah yang terpadu guna menciptakan lingkungan desa yang bersih dan sehat.
                        </p>
                    </div>
                </div>

                <div class="bg-surface-card rounded-xl overflow-hidden border border-hairline group cursor-pointer shadow-sm hover:shadow-md transition-shadow">
                    <div class="aspect-[4/3] overflow-hidden bg-surface-soft relative">
                        <img 
                            src="/assets/626a9203-935b-4782-b12c-91d17ad4ea31.JPG.jpeg" 
                            alt="Ketahanan Pangan" 
                            class="w-full h-full object-cover transition-transform duration-700 group-hover:scale-105"
                            onerror={(e) => { e.currentTarget.src='https://images.unsplash.com/photo-1542838132-92c53300491e?w=800&q=80'; e.currentTarget.onerror=null; }}
                        />
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-medium text-ink mb-2">Ketahanan Pangan</h3>
                        <p class="text-body text-sm leading-relaxed">
                            Optimalisasi lahan dan distribusi sarana produksi pertanian untuk menyokong stabilitas pangan warga, menjamin ketersediaan bahan pokok secara berkelanjutan.
                        </p>
                    </div>
                </div>

                <div class="bg-surface-card rounded-xl overflow-hidden border border-hairline group cursor-pointer shadow-sm hover:shadow-md transition-shadow">
                    <div class="aspect-[4/3] overflow-hidden bg-surface-soft relative">
                        <img 
                            src="/assets/IMG20260620115039.jpg.jpeg" 
                            alt="Pusat Study" 
                            class="w-full h-full object-cover transition-transform duration-700 group-hover:scale-105"
                            onerror={(e) => { e.currentTarget.src='https://images.unsplash.com/photo-1542838132-92c53300491e?w=800&q=80'; e.currentTarget.onerror=null; }}
                        />
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-medium text-ink mb-2">Pusat Study</h3>
                        <p class="text-body text-sm leading-relaxed">
                            Fasilitas edukasi dan pelatihan untuk meningkatkan kapasitas SDM desa, membekali generasi muda dengan pengetahuan dan keterampilan modern.
                        </p>
                    </div>
                </div>

                <div class="bg-surface-card rounded-xl overflow-hidden border border-hairline group cursor-pointer shadow-sm hover:shadow-md transition-shadow">
                    <div class="aspect-[4/3] overflow-hidden bg-surface-soft relative">
                        <img 
                            src="/assets/bumdes1.png" 
                            alt="Kolam Renang" 
                            class="w-full h-full object-cover transition-transform duration-700 group-hover:scale-105"
                            onerror={(e) => { e.currentTarget.src='https://images.unsplash.com/photo-1542838132-92c53300491e?w=800&q=80'; e.currentTarget.onerror=null; }}
                        />
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-medium text-ink mb-2">Kolam Renang</h3>
                        <p class="text-body text-sm leading-relaxed">
                            Unit usaha pariwisata yang menawarkan sarana rekreasi keluarga yang nyaman dan aman, sekaligus menjadi sumber pendapatan asli desa.
                        </p>
                    </div>
                </div>

                <div class="bg-surface-card rounded-xl overflow-hidden border border-hairline group cursor-pointer shadow-sm hover:shadow-md transition-shadow">
                    <div class="aspect-[4/3] overflow-hidden bg-surface-soft relative">
                        <img 
                            src="/assets/IMG_0597.HEIC" 
                            alt="Living Labolatory Learning" 
                            class="w-full h-full object-cover transition-transform duration-700 group-hover:scale-105"
                            onerror={(e) => { e.currentTarget.src='https://images.unsplash.com/photo-1542838132-92c53300491e?w=800&q=80'; e.currentTarget.onerror=null; }}
                        />
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-medium text-ink mb-2">Living Labolatory Learning</h3>
                        <p class="text-body text-sm leading-relaxed">
                            Konsep pembelajaran inovatif berbasis lingkungan hidup yang menjadikan desa sebagai laboratorium nyata untuk penelitian dan edukasi bagi berbagai kalangan masyarakat.
                        </p>
                    </div>
                </div>

                <div class="bg-surface-card rounded-xl overflow-hidden border border-hairline group cursor-pointer shadow-sm hover:shadow-md transition-shadow">
                    <div class="aspect-[4/3] overflow-hidden bg-surface-soft relative">
                        <img 
                            src="/assets/IMG_0602.HEIC" 
                            alt="Taman Tasunting" 
                            class="w-full h-full object-cover transition-transform duration-700 group-hover:scale-105"
                            onerror={(e) => { e.currentTarget.src='https://images.unsplash.com/photo-1542838132-92c53300491e?w=800&q=80'; e.currentTarget.onerror=null; }}
                        />
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-medium text-ink mb-2">Taman Tasunting</h3>
                        <p class="text-body text-sm leading-relaxed">
                            Ruang terbuka hijau yang dikelola untuk menunjang aktivitas sosial budaya dan ekowisata, mempercantik estetika desa, serta menjadi wadah interaksi positif warga.
                        </p>
                    </div>
                </div>

            </div>
        </section>

    </div>
</main>
