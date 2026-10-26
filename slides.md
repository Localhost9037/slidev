---
theme: default
title: Guerra Fria
info: |
  ## Slides sobre a Guerra Fria

  Apresentação sobre a Guerra Fria.
class: text-center flex flex-col justify-center items-center h-full
drawings:
  persist: false
transition: slide-up
comark: true
duration: 10min
level: 1
---
<!-- Background Layer 1: Initial Gradient (Visible by default, fades out on click 2+) -->
<div
  class="fixed inset-0 -z-10 bg-cover bg-center transition-opacity duration-700"
  :class="$clicks > 1 ? 'opacity-0' : 'opacity-100'"
  style="background: linear-gradient(135deg, #a832a8 0%, #571a57 55%, #000000 100%);"
/>

<!-- Background Layer 2: Target Gradient (Hidden by default, fades in on click 2+) -->
<div
  class="fixed inset-0 -z-10 bg-cover bg-center transition-opacity duration-700"
  :class="$clicks > 1 ? 'opacity-100' : 'opacity-0'"
  style="background: linear-gradient(to right, #0A3161 0%, #0A3161 36%, #777783 48%, #99949A 52%, #C50000 64%, #C50000 100%);"
/>
<div v-motion :initial="{ opacity: 1 }" :click-2="{ opacity: 0, transition: { duration: 500 } }">
  
  <h1> Bem-vindo á nossa apresentação </h1>
  <div v-click class="mt-8">
  <span class="font-semibold text-lg opacity-90">
    Participantes:
  </span>

  <div class="mt-3 space-y-2 text-md">
    <p>Caio Muglia</p>
    <p>Yohas Gama</p>
    <p>Matheus Teles</p>
    <p>
      Kauã Massariol
    </p>
  </div>
</div>
</div>

<div v-click.fadein="2" :enter="{ opacity: 1, transition: { duration: 500 } }" class="font-bold">
  <h1 class=" text-gray-400"> Guerra fria </h1>

  <div class="absolute left-[40vw] top-[20px] w-[10vw]" style="transform: rotate(-0deg);">
      <svg 
        version="1.1" 
        xmlns="http://www.w3.org/2000/svg" 
        viewBox="0 0 122.88 122.44" 
        class="w-full h-full fill-current text-amber-600"
      >
        <style>
          .st0 { fill-rule: evenodd; clip-rule: evenodd; }
        </style>
        <g>
          <path class="st0" d="M50.14,42.06l39.38,37.6C107.96,56.04,88.92,15.88,61.27,0c41.32,9.42,65.89,58.63,42.23,92.52l17.75,16.87 c5.75,6.5-5.04,17.12-12.41,11.44l-16.7-18.12c-22.17,10-41.35,5.93-55.09-10.11c-0.34,2.18-2.33,3.69-4.92,5.31 c-6.12,3.84-8.02,7.07-9.27,9.99c-0.84,1.96-1.38,3.78-2.7,5.55c-4.09,5.46-8.33,9.51-15.44,8.54c-2.8,0.85-5.06-0.76-4.45-3.48 c-1.51-6.83,3.42-14.05,10.86-17.91c2.33-1.21,4.47-1.75,6.74-3.21c0.87-0.56,1.67-1.17,2.37-1.88c5.01-5.11,3.75-6.61,6.51-9.04 c0.96-0.85,2.08-1.36,3.39-1.42c0.95-1.46,3.13-2.47,5.62-1.6l3.36-2.86c11.66,11.96,25.97,12.95,39.02,7.77L41.68,50.65 L27.29,64.77L11.98,49.44l30.59-30.29l26.76,3.86L50.14,42.06L50.14,42.06z"/>
        </g>
      </svg>
    </div>
    <div class="absolute left-[0vw] top-[20px] w-[10vw]" style="transform: rotate(4deg);" >
      <svg 
        xmlns="http://www.w3.org/2000/svg" 
        viewBox="0 0 31.371 31.371" 
        class="w-full h-full fill-current text-amber-600"
      >
        <g>
          <path d="M24.26,20.34c0,3.42-2.423,6.342-6.845,7.111v3.92h-3.768v-3.648c-2.578-0.117-5.076-0.811-6.537-1.654l1.154-4.5 c1.615,0.886,3.883,1.693,6.383,1.693c2.191,0,3.691-0.848,3.691-2.385c0-1.461-1.23-2.389-4.077-3.348 c-4.112-1.385-6.921-3.306-6.921-7.033c0-3.386,2.385-6.035,6.499-6.845V0h3.767v3.383c2.576,0.115,4.309,0.652,5.576,1.268 l-1.115,4.348C21.07,8.575,19.3,7.688,16.531,7.688c-2.5,0-3.307,1.076-3.307,2.154c0,1.268,1.346,2.074,4.613,3.307 C22.416,14.762,24.26,16.877,24.26,20.34z"/>
        </g>
      </svg>
    </div>
</div>
---
transition: slide-up
level: 2
---

<style>
.slidev-layout {
  background: linear-gradient(to right, #0A3161 0%, #0A3161 36%, #777783 48%, #99949A 52%, #C50000 64%, #C50000 100%);
}
</style>
<div class="text-center text-gray-400 drop-shadow-[0_5px_5px_rgba(0,0,0,0.8)]">
  <p class="text-4xl">Motivos pelo início</p>
</div>

<div class="flex gap-6 mt-8">
  <!-- Coluna 1 -->
  <div v-click v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1, transition: { duration: 1000 } }" class="w-1/3 p-4 bg-gray-800 rounded-lg h-[40vh]">
    <div class="text-amber-400 font-bold text-lg">O Conflito</div>
    <div class="text-xs text-gray-400 mb-3">1947 a 1991</div>
    <ul class="list-disc list-inside space-y-2 text-sm text-gray-300">
      <li><strong>Natureza:</strong> Conflito político, econômico e ideológico (sem confronto militar direto).</li>
      <li><strong>Polarização:</strong> Dividiu o mundo em Capitalismo (EUA) e Socialismo (URSS).</li>
    </ul>
  </div>
  
  <!-- Coluna 2 -->
  <div v-click v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1, transition: { duration: 1000 } }" class="w-1/3 p-4 bg-gray-800 rounded-lg h-[40vh]">
    <div class="text-amber-400 font-bold text-lg">A Reação dos EUA</div>
    <div class="text-xs text-gray-400 mb-3">1947 em diante</div>
    <ul class="list-disc list-inside space-y-2 text-sm text-gray-300">
      <li><strong>Doutrina Truman:</strong> Promessa de apoiar nações livres e conter o comunismo.</li>
      <li><strong>Plano Marshall:</strong> Ajuda financeira para reconstruir a Europa e mantê-la capitalista.</li>
    </ul>
  </div>
  
  <!-- Coluna 3 -->
  <div v-click v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1, transition: { duration: 1000 } }" class="w-1/3 p-4 bg-gray-800 rounded-lg h-[40vh]">
    <div class="text-amber-400 font-bold text-lg">A Resposta da URSS</div>
    <div class="text-xs text-gray-400 mb-3">1947 a 1949</div>
    <ul class="list-disc list-inside space-y-2 text-sm text-gray-300">
      <li><strong>Comecon:</strong> Bloco econômico para integrar a Europa Oriental.</li>
      <li><strong>Cominform:</strong> Órgão para fortalecer o comunismo e afastar os EUA.</li>
    </ul>
  </div>
</div>
---
transition: slide-up
level: 3
---
<style>
.slidev-layout {
  background: linear-gradient(to right, #0A3161 0%, #0A3161 36%, #777783 48%, #99949A 52%, #C50000 64%, #C50000 100%);
}
</style>

<div class="flex h-full items-center gap-8">    
  <!-- 1/3 Column (Left) -->
  <div class="w-1/3">
    <div class="text-3xl font-bold text-gray-200 drop-shadow-[0_10px_10px_rgba(0,0,0,0.8)]">Bipolaridade e Alianças</div>
    <div class="text-sm text-gray-400 mt-2">O mundo dividido em blocos</div>
  </div>
  <!-- 2/3 Column (Right) -->
  <div class="w-2/3 flex flex-col gap-4">
    <div class="p-4 rounded-lg bg-gray-800/50 border border-gray-700/50 text-gray-300 text-xl shadow-[0_5px_5px_rgba(0,0,0,0.8)]" v-click>
      <strong>A Ordem Bipolar:</strong> Divisão global entre a influência capitalista (EUA) e socialista (URSS).
    </div>     
    <div class="p-4 rounded-lg bg-gray-800/50 border border-gray-700/50 text-gray-300 text-xl shadow-[0_5px_5px_rgba(0,0,0,0.8)]" v-click>
      <strong>OTAN (1949):</strong> Aliança militar ocidental para defesa mútua dos países capitalistas.
    </div>
    <div class="p-4 rounded-lg bg-gray-800/50 border border-gray-700/50 text-gray-300 text-xl shadow-[0_5px_5px_rgba(0,0,0,0.8)]" v-click>
      <strong>Pacto de Varsóvia (1955):</strong> Bloco militar de resposta liderado pela União Soviética no Leste Europeu.
    </div>         
  </div>
</div>



---
transition: slide-up
level: 4
---
<style>
.slidev-layout {
  background: linear-gradient(to right, #0A3161 0%, #0A3161 36%, #777783 48%, #99949A 52%, #C50000 64%, #C50000 100%);
}
</style>

<div class="text-center text-gray-400 drop-shadow-[0_5px_5px_rgba(0,0,0,0.8)]">
  <p class="text-4xl">Corrida armamentista e espacial</p>
</div>
<br />
<br />
<br />


<div class="relative w-full h-full">
  <!-- Step 1: Bombas nucleares -->
  <div v-click class="text-center text-gray-400 drop-shadow-[0_5px_5px_rgba(0,0,0,0.8)] my-4">
    <p class="text-2xl">Bombas nucleares</p>
  </div>
  
  <!-- Step 2: MAD Text -->
  <div v-click class="text-center text-gray-400 drop-shadow-[0_5px_5px_rgba(0,0,0,0.8)] my-4">
    <p class="text-2xl">MAD (Mutually Assured Destruction)</p>
  </div>

  <!-- Step 2 Icon (Appears simultaneously with MAD using v-after or matching click index) -->
  <div v-after class="absolute left-[1vw] top-[-10vh] w-[8vw]">
    <svg 
      version="1.1" 
      id="icon_mad" 
      xmlns="http://www.w3.org/2000/svg" 
      viewBox="0 0 25.979 25.979" 
      class="w-full h-full fill-current text-amber-600"
    >
      <g>
        <path d="M25.744,6.604C26.08,6.267,26.107,6.02,25.48,6.02c-0.628,0-4.556,0-5.068,0  c-0.512,0-0.533,0.016-0.814,0.297c-0.281,0.281-4.604,4.607-4.604,4.607s5.413,0,5.877,0c0.465,0,0.633-0.037,0.912-0.318  C22.063,10.326,25.408,6.94,25.744,6.604z"/>
        <path d="M19.375,0.235c0.336-0.335,0.584-0.363,0.584,0.264s0,4.555,0,5.067S19.943,6.1,19.662,6.381  s-4.607,4.604-4.607,4.604s0-5.414,0-5.878c0-0.464,0.037-0.632,0.318-0.912C15.653,3.916,19.039,0.571,19.375,0.235z"/>
        <path d="M1.621,16.53c-2.161,2.162-2.162,5.666-0.001,7.828c2.161,2.161,5.667,2.161,7.828,0  c0.93-0.931,6.001-6,6.931-6.93c2.161-2.161,2.161-5.666,0-7.829c-2.162-2.162-5.666-2.161-7.828,0  C7.621,10.531,2.551,15.6,1.621,16.53z"/>
      </g>
    </svg>
  </div>

  <!-- Step 3: Corrida espacial -->
  <div v-click class="text-center text-gray-400 drop-shadow-[0_5px_5px_rgba(0,0,0,0.8)] my-4">
    <p class="text-2xl">Corrida espacial</p>
  </div>
    
  <!-- Step 4: Vitória estadunidense Text -->
  <div v-click class="text-center text-gray-400 drop-shadow-[0_5px_5px_rgba(0,0,0,0.8)] my-4">
    <p class="text-2xl">Vitória estadunidense</p>
  </div>

  <!-- Step 4 Icon (Appears simultaneously with Vitória estadunidense) -->
  <div v-after class="absolute left-[39vw] top-[-10vh] w-[8vw]">
    <svg 
      version="1.1" 
      id="Layer_1" 
      xmlns="http://www.w3.org/2000/svg" 
      viewBox="0 0 121.12 122.88" 
      class="w-full h-full fill-current text-amber-600"
    >
      <g>
        <path d="M9.61,114.81c3.99,4.34,12.59,2.3,23.22-3.61c-9.67-6.54-17.2-15.98-21.36-27.08C5.18,96.93,3.53,108.18,9.61,114.81 L9.61,114.81z M110.6,31.4c4.88-9.62,6.38-17.43,2.66-21.51c-5.71-6.25-16.44-4.79-28.96,1.33C94.95,15.2,104.09,22.3,110.6,31.4 L110.6,31.4z M64.51,7.67c3.96,0,7.83,0.41,11.56,1.18c17.19-9.68,32.87-12.5,41.58-2.97c5.6,6.13,3.67,17.02-2.89,29.78l0-0.01 l-0.03,0.07c-0.21,0.41-0.42,0.81-0.64,1.23l0.05,0.1c-14.06,31.09-41.39,57.46-73.32,76.33l-2.11,1.32l-0.05-0.03 c-14.46,8.49-26.94,11.28-33.45,4.19c-8.83-9.62-5.73-25.63,3.9-42.84C8.32,72.22,7.9,68.3,7.9,64.28 C7.9,33.01,33.24,7.67,64.51,7.67L64.51,7.67z M118.62,47.6c1.62,5.27,2.5,10.87,2.5,16.68c0,31.26-25.34,56.61-56.61,56.61 c-5.86,0-11.51-0.89-16.82-2.54c31.51-18.76,55.43-42.16,70.92-70.72l0,0L118.62,47.6L118.62,47.6z"/>
      </g>
    </svg>
  </div>
</div>
---
transition: slide-up
level: 5
---
<style>
.slidev-layout {
  background: linear-gradient(to right, #0A3161 0%, #0A3161 36%, #777783 48%, #99949A 52%, #C50000 64%, #C50000 100%);
}
</style>

<div class="flex h-full items-center gap-8">    
  <!-- 1/3 Column (Left) -->
  <div class="w-1/3">
    <div class="text-3xl font-bold text-gray-200 drop-shadow-[0_10px_10px_rgba(0,0,0,0.8)]" >Conflitos indiretos</div>
    <div class="text-sm text-gray-400 mt-2"></div> <br /><br /><br /><br /><br /><br /><br /><br /><br /><br />
  </div>
  <!-- 2/3 Column (Right) -->
  <div class="w-2/3 flex flex-col gap-4">
    <div class="p-4 rounded-lg bg-gray-800/50 border border-gray-700/50 text-gray-300 text-2xl shadow-[0_5px_5px_rgba(0,0,0,0.8)]" v-click >
      Revolução Cubana
    </div>     
    <div class="p-4 rounded-lg bg-gray-800/50 border border-gray-700/50 text-gray-300 text-2xl shadow-[0_5px_5px_rgba(0,0,0,0.8)]" v-click >
      Guerra do Vietnã
    </div>
    <div class="p-4 rounded-lg bg-gray-800/50 border border-gray-700/50 text-gray-300 text-2xl shadow-[0_5px_5px_rgba(0,0,0,0.8)]" v-click >
      Guerra da Coreia
    </div>        
    <div class="p-4 rounded-lg bg-gray-800/50 border border-gray-700/50 text-gray-300 text-2xl shadow-[0_5px_5px_rgba(0,0,0,0.8)]" v-click >
      Guerra do Afeganistão
    </div>
  </div>
</div>

---
transition: slide-up
level: 6
---
<style>
.slidev-layout {
  background: linear-gradient(to right, #0A3161 0%, #0A3161 36%, #777783 48%, #99949A 52%, #C50000 64%, #C50000 100%);
}
</style>

<div class="flex h-full items-center gap-8">    
  <!-- 1/3 Column (Left) -->
  <div class="w-1/3">
    <div class="text-3xl font-bold text-gray-200 drop-shadow-[0_10px_10px_rgba(0,0,0,0.8)]">Símbolos da Divisão</div>
    <div class="text-sm text-gray-400 mt-2">A materialização da Cortina de Ferro</div>
  </div>
  <!-- 2/3 Column (Right) -->
  <div class="w-2/3 flex flex-col gap-4">
    <div class="p-4 rounded-lg bg-gray-800/50 border border-gray-700/50 text-gray-300 text-xl shadow-[0_5px_5px_rgba(0,0,0,0.8)]" v-click>
      <strong>O Muro de Berlim:</strong> Construído em 1961, separou fisicamente famílias e ideologias na capital alemã.
    </div>     
    <div class="p-4 rounded-lg bg-gray-800/50 border border-gray-700/50 text-gray-300 text-xl shadow-[0_5px_5px_rgba(0,0,0,0.8)]" v-click>
      <strong>A Cortina de Ferro:</strong> Termo popularizado por Winston Churchill para definir a fronteira ideológica da Europa.
    </div>     
  </div>
</div>

---
transition: slide-up
level: 6
---
<style>
.slidev-layout {
  background: linear-gradient(to right, #0A3161 0%, #0A3161 36%, #777783 48%, #99949A 52%, #C50000 64%, #C50000 100%);
}
</style>

<div class="text-center text-gray-400 drop-shadow-[0_5px_5px_rgba(0,0,0,0.8)]">
  <p class="text-4xl">Desfecho da Guerra Fria</p>
</div>

<div class="flex gap-6 mt-8">
  <!-- Coluna 1 -->
  <div v-click v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1, transition: { duration: 1000 } }" class="w-1/3 p-4 bg-gray-800 rounded-lg h-[40vh]">
    <div class="text-amber-400 font-bold text-lg">Crise na URSS</div>
    <div class="text-xs text-gray-400 mb-3">Década de 1980</div>
    <ul class="list-disc list-inside space-y-2 text-sm text-gray-300">
      <li><strong>Glasnost:</strong> Transparência política e liberdade de expressão.</li>
      <li><strong>Perestroika:</strong> Reestruturação econômica e abertura parcial ao mercado.</li>
    </ul>
  </div>
  
  <!-- Coluna 2 -->
  <div v-click v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1, transition: { duration: 1000 } }" class="w-1/3 p-4 bg-gray-800 rounded-lg h-[40vh]">
    <div class="text-amber-400 font-bold text-lg">Queda do Muro</div>
    <div class="text-xs text-gray-400 mb-3">Novembro de 1989</div>
    <ul class="list-disc list-inside space-y-2 text-sm text-gray-300">
      <li><strong>Fim da divisão:</strong> Abertura das fronteiras e unificação alemã em 1990.</li>
      <li><strong>Fim simbólico:</strong> O colapso do bloco comunista na Europa Oriental.</li>
    </ul>
  </div>
  
  <!-- Coluna 3 -->
  <div v-click v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1, transition: { duration: 1000 } }" class="w-1/3 p-4 bg-gray-800 rounded-lg h-[40vh]">
    <div class="text-amber-400 font-bold text-lg">Fim da URSS</div>
    <div class="text-xs text-gray-400 mb-3">Dezembro de 1991</div>
    <ul class="list-disc list-inside space-y-2 text-sm text-gray-300">
      <li><strong>Dissolução:</strong> Fim oficial da União Soviética.</li>
      <li><strong>Nova ordem:</strong> Vitória do capitalismo e início do mundo unipolar liderado pelos EUA.</li>
    </ul>
  </div>
</div>

---
transition: slide-up
level: 7
---

<!-- Background Layer 1: Initial Gradient (Visible by default, fades out on click 2+) -->
<div
  class="fixed inset-0 -z-10 bg-cover bg-center transition-opacity duration-700"
  :class="$clicks > 0 ? 'opacity-100' : 'opacity-0'"
  style="background: linear-gradient(135deg, #a832a8 0%, #571a57 55%, #000000 100%);"
/>

<!-- Background Layer 2: Target Gradient (Hidden by default, fades in on click 2+) -->
<div
  class="fixed inset-0 -z-10 bg-cover bg-center transition-opacity duration-700"
  :class="$clicks > 0 ? 'opacity-0' : 'opacity-100'"
  style="background: linear-gradient(to right, #0A3161 0%, #0A3161 36%, #777783 48%, #99949A 52%, #C50000 64%, #C50000 100%);"
/>
<div v-click />
<div v-motion absolute inset-0 :initial="{ opacity: 1 }" :click-1="{ opacity: 0, transition: { duration: 500 } }"> 
  <div class="text-3xl font-bold text-gray-200 drop-shadow-[0_10px_10px_rgba(0,0,0,0.8)] text-center">
     <p>Hora de pensar</p>
     <img class="w-1/2 h-1/2 mx-auto block rounded-lg"
     src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhj_TEs9iptMJM1q_k7Q5GZTqoib4ENvnortpTQU1v38OBzK8VqHzHV5tpK45Q8GGyo6tBdcNFunPNVPq0qqrpGCVES13IFbnbmpAj2CnGbOFJ9hLe57pUSnNnDcgkW41LuRyjBwUWcXd-n5A-AAPFjOKnZeXryvDt6g50h8uGwtWeaQs7HHWGFPvJmQQ/w640-h548/Charge%20pelada.jpg">
  </div>
</div>

<div v-motion absolute inset-0 :initial="{ opacity: 0 }" :click-1="{ opacity: 1, transition: { duration: 500 } }"> 
<br /><br /><br />
   <div class="text-3xl font-bold text-gray-200 drop-shadow-[0_10px_10px_rgba(0,0,0,0.8)] text-center">  
     <p> Obrigado pela atenção! </p>
   </div>
   <br /><br /><br /><br /><br />
    <div class="text-xl text-gray-400 drop-shadow-[0_10px_10px_rgba(0,0,0,0.8)] text-center">  
     <p> Fontes: Toda matéria, Brasil Escola, material SAS </p>
   </div>
</div>
