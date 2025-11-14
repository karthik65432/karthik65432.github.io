---
layout: default
title: "Karthik K — GenAI Engineer · Product Manager · Design Thinker"
---

# 👋 Hi, I’m Karthik K
GenAI Engineer · Product Manager · Design Thinker  
I build next-generation AI systems that merge product vision, model design, and user empathy into scalable solutions.

---

<h2 class="section-title mt-16 mb-8">
  🧠 Skills
</h2>

<div id="skills" class="grid sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-6 mt-6">
{% for skill in site.data.skills %}
  <div class="ai-card p-5 rounded-2xl text-center font-semibold flex flex-col items-center gap-2">
    <img src="/assets/icons/{{ skill.icon }}" alt="{{ skill.name }}" class="w-8 h-8">
    <span>{{ skill.name }}</span>
  </div>
{% endfor %}
</div>

---

<h2 class="section-title mt-16 mb-8">
  🎓 Education & Languages
</h2>
<div id="education" class="space-y-10 mt-10">
{% for edu in site.data.education %}
  <div class="ai-card border border-slate-200 bg-slate-50 p-6 rounded-2xl flex items-center gap-4">
    <img src="/assets/icons/{{ edu.logo }}" alt="{{ edu.school }}" class="w-14 h-14 rounded-md border border-slate-300 p-1 bg-white">
    <div>
      <h3 class="font-semibold text-lg">{{ edu.school }}</h3>
      {% if edu.year %}<p class="text-sm text-slate-500">{{ edu.year }}</p>{% endif %}
      <p>{{ edu.degree }}</p>
      {% if edu.award %}<p class="mt-1 text-emerald-600 text-sm">{{ edu.award }}</p>{% endif %}
    </div>
  </div>
{% endfor %}
</div>

---


<h2 class="section-title mt-16 mb-8">
  💼 Experience
</h2>

<div id="experience" class="grid md:grid-cols-3 gap-6 mt-10 justify-items-center">
{% for job in site.data.experience %}
  <div class="ai-card max-w-sm w-full mx-auto p-8 rounded-3xl shadow-deep text-center flex flex-col items-center justify-between">
    <img src="/assets/icons/{{ job.logo }}" alt="{{ job.company }}" class="w-20 h-20 mb-4 object-contain rounded-lg">
    <h3 class="text-xl font-bold">{{ job.company }}</h3>
    <p class="text-sm text-slate-500 mb-2">{{ job.period }} | {{ job.role }}</p>
    <p class="text-sm text-slate-700">{{ job.description }}</p>
  </div>
{% endfor %}
</div>


---

<h2 class="section-title mt-16 mb-8">
  🏆 Awards
</h2>
<div id="awards" class="grid md:grid-cols-3 gap-6 mt-10">
{% for award in site.data.awards %}
  <div class="ai-card p-6 rounded-2xl text-center flex flex-col items-center">
    <img src="/assets/icons/{{ award.icon }}" alt="{{ award.name }}" class="w-10 h-10 mb-3">
    <h3 class="font-semibold">{{ award.name }}</h3>
    <p class="text-sm text-slate-500">{{ award.date }}</p>
    <p class="text-sm mt-2">{{ award.description }}</p>
  </div>
{% endfor %}
</div>

---


<h2 class="section-title mt-16 mb-8">
  🚀 Projects
</h2>
<div id="projects" class="grid md:grid-cols-2 lg:grid-cols-3 gap-6 mt-10">
{% for project in site.data.projects %}
  <div class="ai-card p-6 rounded-2xl overflow-hidden">
    <img src="/assets/icons/{{ project.image }}" alt="{{ project.title }}" class="w-full h-48 object-cover rounded-xl mb-4">
    <h3 class="font-semibold text-lg">{{ project.title }}</h3>
    <p class="text-sm text-slate-500 mt-2">{{ project.description }}</p>
  </div>
{% endfor %}
</div>

