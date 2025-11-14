---
layout: default
title: "Karthik K — GenAI Engineer · Product Manager · Design Thinker"
---

<!-- Hero Section - Side by Side Layout -->
<section class="min-h-screen flex items-center py-20 px-4">
  <div class="max-w-7xl mx-auto w-full">
    <div class="grid lg:grid-cols-2 gap-12 lg:gap-20 items-center">
      
      <!-- Left: Text Content -->
      <div class="space-y-8 scroll-reveal">
        <div class="inline-block px-4 py-2 bg-brand-50 rounded-full text-brand-600 text-sm font-semibold mb-4">
          👋 Welcome to my portfolio
        </div>
        
        <h1 class="text-5xl md:text-6xl lg:text-7xl font-display font-bold text-slate-900 leading-tight">
          Hi, I'm <span class="gradient-text">Karthik K</span>
        </h1>
        
        <p class="text-2xl md:text-3xl text-brand-600 font-semibold">
          GenAI Engineer · Product Manager · Design Thinker
        </p>
        
        <p class="text-lg md:text-xl text-slate-600 leading-relaxed max-w-2xl">
          I build next-generation AI systems that merge product vision, model design, and user empathy into scalable solutions.
        </p>
        
        <div class="flex flex-wrap gap-4 pt-4">
          <a href="#experience" class="px-8 py-4 bg-brand-600 text-white rounded-full font-semibold hover:bg-brand-700 transition-all hover:scale-105 shadow-medium hover:shadow-strong">
            View My Work
          </a>
          <a href="#contact" class="px-8 py-4 bg-white text-brand-600 border-2 border-brand-600 rounded-full font-semibold hover:bg-brand-50 transition-all hover:scale-105">
            Get In Touch
          </a>
        </div>
      </div>
      
      <!-- Right: Large Profile Image Placeholder -->
      <div class="scroll-reveal">
        <div class="relative">
          <!-- Decorative background elements -->
          <div class="absolute -top-10 -right-10 w-72 h-72 bg-brand-100 rounded-full blur-3xl opacity-50 animate-pulse"></div>
          <div class="absolute -bottom-10 -left-10 w-64 h-64 bg-blue-100 rounded-full blur-3xl opacity-50 animate-pulse" style="animation-delay: 1s;"></div>
          
          <!-- Profile image container - large jazzy tile -->
          <div class="relative z-10 aspect-square max-w-lg mx-auto">
            <div class="w-full h-full rounded-3xl overflow-hidden shadow-strong border-4 border-white">
              <img src="/assets/icons/karthik_passport.jpg" 
                   alt="Karthik K" 
                   class="w-full h-full object-cover hover:scale-105 transition-transform duration-700" />
            </div>
            
            <!-- Floating badge -->
            <div class="absolute -bottom-6 -right-6 bg-white rounded-2xl shadow-strong p-6 border border-slate-100">
              <div class="text-center">
                <div class="text-3xl font-bold text-brand-600">5+</div>
                <div class="text-sm text-slate-600 font-medium">Years Experience</div>
              </div>
            </div>
          </div>
        </div>
      </div>
      
    </div>
  </div>
</section>

<!-- Skills Section - Modern Grid -->
<section id="skills" class="py-20 px-4 bg-gradient-to-b from-white to-slate-50">
  <div class="max-w-7xl mx-auto">
    <div class="text-center mb-16 scroll-reveal">
      <h2 class="section-title">🧠 Skills & Expertise</h2>
      <p class="text-xl text-slate-600 max-w-2xl mx-auto">
        A comprehensive toolkit for building intelligent systems at scale
      </p>
    </div>
    
    <div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 xl:grid-cols-6 gap-4 md:gap-6">
      {% for skill in site.data.skills %}
      <div class="skill-badge text-center group scroll-reveal">
        <img src="/assets/icons/{{ skill.icon }}" 
             alt="{{ skill.name }}" 
             class="w-12 h-12 mx-auto mb-3 group-hover:scale-110 transition-transform duration-300" />
        <div class="font-semibold text-slate-700 group-hover:text-brand-600 transition-colors">
          {{ skill.name }}
        </div>
      </div>
      {% endfor %}
    </div>
  </div>
</section>

<!-- Experience Section - Bento Grid Style -->
<section id="experience" class="py-20 px-4">
  <div class="max-w-7xl mx-auto">
    <div class="mb-16 scroll-reveal">
      <h2 class="section-title">💼 Professional Experience</h2>
      <p class="text-xl text-slate-600 max-w-2xl">
        Driving AI innovation across Fortune 500 companies
      </p>
    </div>
    
    <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-6">
      {% for job in site.data.experience %}
      <div class="modern-card group cursor-pointer scroll-reveal">
        <!-- Company Logo -->
        <div class="w-16 h-16 mb-6 p-3 bg-slate-50 rounded-2xl group-hover:bg-brand-50 transition-colors">
          <img src="/assets/icons/{{ job.logo }}" 
               alt="{{ job.company }}" 
               class="w-full h-full object-contain" />
        </div>
        
        <!-- Content -->
        <h3 class="text-xl font-bold text-slate-900 mb-2 group-hover:text-brand-600 transition-colors">
          {{ job.company }}
        </h3>
        <div class="text-brand-600 font-semibold mb-1">{{ job.role }}</div>
        <div class="text-sm text-slate-500 mb-4">{{ job.period }}</div>
        <p class="text-slate-600 leading-relaxed">{{ job.description }}</p>
      </div>
      {% endfor %}
    </div>
  </div>
</section>

<!-- Education Section - Horizontal Scroll Cards -->
<section id="education" class="py-20 px-4 bg-gradient-to-b from-slate-50 to-white">
  <div class="max-w-7xl mx-auto">
    <div class="mb-16 scroll-reveal">
      <h2 class="section-title">🎓 Education & Languages</h2>
      <p class="text-xl text-slate-600">Academic foundation and linguistic capabilities</p>
    </div>
    
    <div class="space-y-4">
      {% for edu in site.data.education %}
      <div class="modern-card flex items-center gap-6 group scroll-reveal">
        <div class="flex-shrink-0">
          <div class="w-16 h-16 p-3 bg-slate-50 rounded-2xl group-hover:bg-brand-50 transition-colors">
            <img src="/assets/icons/{{ edu.logo }}" 
                 alt="{{ edu.school }}" 
                 class="w-full h-full object-contain" />
          </div>
        </div>
        
        <div class="flex-grow">
          <h3 class="text-lg font-bold text-slate-900 group-hover:text-brand-600 transition-colors">
            {{ edu.school }}
          </h3>
          {% if edu.year %}
          <div class="text-sm text-slate-500 mb-1">{{ edu.year }}</div>
          {% endif %}
          <div class="text-slate-700">{{ edu.degree }}</div>
          {% if edu.award %}
          <div class="mt-2 inline-block px-3 py-1 bg-emerald-50 text-emerald-700 text-sm rounded-full font-medium">
            ✨ {{ edu.award }}
          </div>
          {% endif %}
        </div>
      </div>
      {% endfor %}
    </div>
  </div>
</section>

<!-- Awards Section - Feature Cards -->
<section id="awards" class="py-20 px-4">
  <div class="max-w-7xl mx-auto">
    <div class="mb-16 scroll-reveal text-center">
      <h2 class="section-title">🏆 Recognition & Awards</h2>
      <p class="text-xl text-slate-600">Celebrating excellence and innovation</p>
    </div>
    
    <div class="grid md:grid-cols-3 gap-6">
      {% for award in site.data.awards %}
      <div class="modern-card text-center group scroll-reveal">
        <div class="w-20 h-20 mx-auto mb-6 p-5 bg-gradient-to-br from-brand-500 to-brand-600 rounded-2xl shadow-glow group-hover:scale-110 transition-transform">
          <img src="/assets/icons/{{ award.icon }}" 
               alt="{{ award.name }}" 
               class="w-full h-full brightness-0 invert" />
        </div>
        
        <h3 class="text-xl font-bold text-slate-900 mb-2">{{ award.name }}</h3>
        <div class="text-brand-600 font-medium mb-3">{{ award.date }}</div>
        <p class="text-slate-600 leading-relaxed">{{ award.description }}</p>
      </div>
      {% endfor %}
    </div>
  </div>
</section>

<!-- Projects Section - Pinterest Style Grid -->
<section id="projects" class="py-20 px-4 bg-gradient-to-b from-white to-slate-50">
  <div class="max-w-7xl mx-auto">
    <div class="mb-16 scroll-reveal">
      <h2 class="section-title">🚀 Featured Projects</h2>
      <p class="text-xl text-slate-600">Transforming ideas into intelligent solutions</p>
    </div>
    
    <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-6">
      {% for project in site.data.projects %}
      <div class="modern-card group cursor-pointer overflow-hidden p-0 scroll-reveal">
        <!-- Image -->
        <div class="relative overflow-hidden aspect-video">
          <img src="/assets/icons/{{ project.image }}" 
               alt="{{ project.title }}" 
               class="w-full h-full object-cover group-hover:scale-110 transition-transform duration-700" />
          <div class="absolute inset-0 bg-gradient-to-t from-black/50 to-transparent opacity-0 group-hover:opacity-100 transition-opacity"></div>
        </div>
        
        <!-- Content -->
        <div class="p-6">
          <h3 class="text-xl font-bold text-slate-900 mb-3 group-hover:text-brand-600 transition-colors">
            {{ project.title }}
          </h3>
          <p class="text-slate-600 leading-relaxed">{{ project.description }}</p>
          
          <div class="mt-4 flex items-center text-brand-600 font-semibold group-hover:gap-2 transition-all">
            <span>Learn more</span>
            <svg class="w-5 h-5 transform group-hover:translate-x-1 transition-transform" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 8l4 4m0 0l-4 4m4-4H3"></path>
            </svg>
          </div>
        </div>
      </div>
      {% endfor %}
    </div>
  </div>
</section>

<!-- Contact Section -->
<section id="contact" class="py-20 px-4">
  <div class="max-w-4xl mx-auto text-center">
    <div class="modern-card p-12 md:p-16 scroll-reveal">
      <h2 class="text-4xl md:text-5xl font-display font-bold text-slate-900 mb-6">
        Let's Build Something <span class="gradient-text">Amazing</span>
      </h2>
      <p class="text-xl text-slate-600 mb-10 max-w-2xl mx-auto">
        Ready to bring your AI vision to life? Let's connect and create intelligent solutions together.
      </p>
      
      <div class="flex flex-wrap justify-center gap-4">
        <a href="mailto:your.email@example.com" 
           class="px-8 py-4 bg-brand-600 text-white rounded-full font-semibold hover:bg-brand-700 transition-all hover:scale-105 shadow-medium flex items-center gap-2">
          <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"></path>
          </svg>
          <span>Email Me</span>
        </a>
        <a href="https://linkedin.com" 
           target="_blank"
           class="px-8 py-4 bg-white text-slate-700 border-2 border-slate-200 rounded-full font-semibold hover:border-brand-600 hover:text-brand-600 transition-all hover:scale-105 flex items-center gap-2">
          <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24">
            <path d="M19 0h-14c-2.761 0-5 2.239-5 5v14c0 2.761 2.239 5 5 5h14c2.762 0 5-2.239 5-5v-14c0-2.761-2.238-5-5-5zm-11 19h-3v-11h3v11zm-1.5-12.268c-.966 0-1.75-.79-1.75-1.764s.784-1.764 1.75-1.764 1.75.79 1.75 1.764-.783 1.764-1.75 1.764zm13.5 12.268h-3v-5.604c0-3.368-4-3.113-4 0v5.604h-3v-11h3v1.765c1.396-2.586 7-2.777 7 2.476v6.759z"/>
          </svg>
          <span>LinkedIn</span>
        </a>
      </div>
    </div>
  </div>
</section>

<!-- Scroll Animation Script -->
<script>
  // Intersection Observer for scroll animations
  const observerOptions = {
    threshold: 0.1,
    rootMargin: '0px 0px -100px 0px'
  };
  
  const observer = new IntersectionObserver((entries) => {
    entries.forEach(entry => {
      if (entry.isIntersecting) {
        entry.target.classList.add('revealed');
      }
    });
  }, observerOptions);
  
  // Observe all elements with scroll-reveal class
  document.querySelectorAll('.scroll-reveal').forEach((el) => {
    observer.observe(el);
  });
</script>
