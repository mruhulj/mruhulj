```aura width=860 height=220
<div style={{
  width: '100%', height: '100%', background: '#0a0a12',
  display: 'flex', flexDirection: 'column', alignItems: 'center', justifyContent: 'center',
  fontFamily: 'Inter, sans-serif', position: 'relative', overflow: 'hidden',
  borderRadius: 20, border: '1px solid rgba(168,85,247,0.14)'
}}>

  <style>{`
    @keyframes h-orb1 { 0%, 100% { transform: translate(0,0); opacity: 0.55; } 50% { transform: translate(35px,-25px); opacity: 0.85; } }
    @keyframes h-orb2 { 0%, 100% { transform: translate(0,0); opacity: 0.45; } 50% { transform: translate(-30px,20px); opacity: 0.75; } }
    @keyframes h-orb3 { 0%, 100% { transform: translate(0,0); opacity: 0.4; } 50% { transform: translate(20px,-15px); opacity: 0.65; } }
    #ho1 { animation: h-orb1 9s ease-in-out infinite; }
    #ho2 { animation: h-orb2 12s ease-in-out infinite 0.6s; }
    #ho3 { animation: h-orb3 10s ease-in-out infinite 1.4s; }
  `}</style>

  <svg width="860" height="220" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="hg1" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(236,72,153,0.42)" />
        <stop offset="60%" stopColor="rgba(236,72,153,0.10)" />
        <stop offset="100%" stopColor="rgba(236,72,153,0)" />
      </radialGradient>
      <radialGradient id="hg2" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(139,92,246,0.48)" />
        <stop offset="55%" stopColor="rgba(139,92,246,0.14)" />
        <stop offset="100%" stopColor="rgba(139,92,246,0)" />
      </radialGradient>
      <radialGradient id="hg3" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(96,165,250,0.35)" />
        <stop offset="100%" stopColor="rgba(96,165,250,0)" />
      </radialGradient>
    </defs>
    <ellipse id="ho1" cx="120" cy="190" rx="260" ry="180" fill="url(#hg1)" />
    <ellipse id="ho2" cx="740" cy="40" rx="240" ry="180" fill="url(#hg2)" />
    <ellipse id="ho3" cx="480" cy="200" rx="200" ry="140" fill="url(#hg3)" />
  </svg>

  <div style={{ position: 'relative', display: 'flex', flexDirection: 'column', alignItems: 'center', zIndex: 10 }}>
    <span style={{
      fontSize: 12, letterSpacing: 5, textTransform: 'uppercase',
      color: 'rgba(216,180,254,0.75)', fontWeight: 600, marginBottom: 16
    }}>UI/UX Designer · Developer</span>

    <div style={{ display: 'flex', fontSize: 44, fontWeight: 400, letterSpacing: -1, lineHeight: 1, color: '#ffffff' }}>
      <span style={{ display: 'flex' }}>Muhammad&nbsp;</span>
      <span style={{ display: 'flex', fontWeight: 800 }}>Ruhul</span>
      <span style={{ display: 'flex' }}>&nbsp;Jadid</span>
    </div>

    <span style={{ fontSize: 16, color: 'rgba(230,225,255,0.75)', fontWeight: 400, marginTop: 14 }}>
      Designing user-centered products — and building the ones I design
    </span>

    <div style={{ display: 'flex', gap: 10, marginTop: 22, flexWrap: 'wrap', justifyContent: 'center' }}>
      {['UI/UX Design', 'Figma', 'Flutter', 'Cloud'].map(function(tag, i) {
        return (
          <span key={i} style={{
            padding: '6px 16px', borderRadius: 100,
            background: 'rgba(168,85,247,0.10)',
            border: '1px solid rgba(168,85,247,0.28)',
            color: 'rgba(230,220,255,0.85)', fontSize: 13, fontWeight: 600, letterSpacing: 0.3
          }}>{tag}</span>
        );
      })}
    </div>
  </div>
</div>
```

```aura width=190 height=52 link="https://linkedin.com/in/mruhulj" inline align=center
<SocialMediaButton
  icon="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/linked-in-alt.svg"
  text="LinkedIn"
  backgroundColor="#0a0a12"
  width={190}
  height={52}
  gradientStops={[
    { offset: '0%', color: '#f472b6' },
    { offset: '50%', color: '#a855f7' },
    { offset: '100%', color: '#6d28d9' },
  ]}
  iconSize="20"
/>
```
```aura width=190 height=52 link="https://mruhulj.carrd.co" inline align=center
<SocialMediaButton
  icon="https://cdn.simpleicons.org/carrd/ffffff"
  text="Portfolio"
  backgroundColor="#0a0a12"
  width={190}
  height={52}
  gradientStops={[
    { offset: '0%', color: '#a855f7' },
    { offset: '50%', color: '#818cf8' },
    { offset: '100%', color: '#60a5fa' },
  ]}
  iconSize="20"
/>
```
```aura width=190 height=52 link="mailto:mruhulj@gmail.com" inline align=center
<SocialMediaButton
  icon="https://cdn.simpleicons.org/gmail/ffffff"
  text="Email"
  backgroundColor="#0a0a12"
  width={190}
  height={52}
  gradientStops={[
    { offset: '0%', color: '#6d28d9' },
    { offset: '50%', color: '#a855f7' },
    { offset: '100%', color: '#f472b6' },
  ]}
  iconSize="20"
/>
```

```aura width=860 height=310
(function() {
 var DEVICON = 'https://cdn.jsdelivr.net/gh/devicons/devicon/icons/';
 var categories = [
   { title: 'Design', color: '#f472b6', items: [
     { name: 'Figma', icon: DEVICON + 'figma/figma-original.svg' },
     { name: 'Canva', icon: DEVICON + 'canva/canva-original.svg' },
   ]},
   { title: 'Mobile & Web', color: '#a78bfa', items: [
     { name: 'Flutter', icon: DEVICON + 'flutter/flutter-original.svg' },
     { name: 'Dart', icon: DEVICON + 'dart/dart-original.svg' },
     { name: 'React', icon: DEVICON + 'react/react-original.svg' },
     { name: 'Node.js', icon: DEVICON + 'nodejs/nodejs-original.svg' },
   ]},
   { title: 'Backend & Cloud', color: '#60a5fa', items: [
     { name: 'Java', icon: DEVICON + 'java/java-original.svg' },
     { name: 'Python', icon: DEVICON + 'python/python-original.svg' },
     { name: 'Google Cloud', icon: DEVICON + 'googlecloud/googlecloud-original.svg' },
     { name: 'MySQL', icon: DEVICON + 'mysql/mysql-original.svg' },
   ]},
 ];

 return (
   <div style={{
     width: '100%', height: '100%', background: '#0a0a12',
     display: 'flex', flexDirection: 'column',
     fontFamily: 'Inter, sans-serif', padding: '26px 40px', gap: 18,
     borderRadius: 20, border: '1px solid rgba(168,85,247,0.14)',
     position: 'relative', overflow: 'hidden',
   }}>

     <style>{`
       @keyframes ts-orb1 { 0%, 100% { transform: translate(0,0); opacity: 0.45; } 50% { transform: translate(30px,-20px); opacity: 0.7; } }
       @keyframes ts-orb2 { 0%, 100% { transform: translate(0,0); opacity: 0.4; } 50% { transform: translate(-25px,15px); opacity: 0.65; } }
       #tso1 { animation: ts-orb1 10s ease-in-out infinite; }
       #tso2 { animation: ts-orb2 13s ease-in-out infinite 1s; }
     `}</style>

     <svg width="860" height="310" style={{ position: 'absolute', top: 0, left: 0 }}>
       <defs>
         <radialGradient id="tsg1" cx="50%" cy="50%" r="50%">
           <stop offset="0%" stopColor="rgba(139,92,246,0.30)" />
           <stop offset="100%" stopColor="rgba(139,92,246,0)" />
         </radialGradient>
         <radialGradient id="tsg2" cx="50%" cy="50%" r="50%">
           <stop offset="0%" stopColor="rgba(236,72,153,0.24)" />
           <stop offset="100%" stopColor="rgba(236,72,153,0)" />
         </radialGradient>
       </defs>
       <ellipse id="tso1" cx="120" cy="290" rx="220" ry="170" fill="url(#tsg1)" />
       <ellipse id="tso2" cx="760" cy="30" rx="200" ry="160" fill="url(#tsg2)" />
     </svg>

     <span style={{ display:'flex', fontSize:11, fontWeight:700, color:'rgba(216,180,254,0.65)', letterSpacing:'4px', zIndex: 10 }}>
       TECH STACK
     </span>

     <div style={{ display:'flex', flexDirection:'column', gap:16, zIndex: 10 }}>
       {categories.map(function(cat) {
         return (
           <div key={cat.title} style={{ display:'flex', flexDirection: 'column', gap:8 }}>
             <div style={{ display:'flex', fontSize:12, fontWeight:700, color:cat.color, letterSpacing:'0.5px' }}>
               {cat.title.toUpperCase()}
             </div>
             <div style={{ display:'flex', flexWrap:'wrap', gap:8 }}>
               {cat.items.map(function(item) {
                 return (
                   <div key={item.name} style={{
                     display:'flex', alignItems:'center', gap:8, padding:'7px 16px 7px 10px', borderRadius:8,
                     background:cat.color + '14', border:'1px solid ' + cat.color + '38',
                   }}>
                     <img src={item.icon} width={17} height={17} />
                     <span style={{ display: 'flex', color:'rgba(240,238,255,0.92)', fontSize:14, fontWeight:600 }}>{item.name}</span>
                   </div>
                 );
               })}
             </div>
           </div>
         );
       })}
     </div>
   </div>
 );
})()
```

```aura width=860 height=210
<div style={{
  width: '100%', height: '100%', background: '#0a0a12',
  display: 'flex', fontFamily: 'Inter, sans-serif',
  position: 'relative', overflow: 'hidden',
  borderRadius: 20, border: '1px solid rgba(96,165,250,0.14)'
}}>

  <style>{`
    @keyframes ab-orb1 { 0%, 100% { transform: translate(0,0); opacity: 0.5; } 50% { transform: translate(25px,-18px); opacity: 0.8; } }
    @keyframes ab-orb2 { 0%, 100% { transform: translate(0,0); opacity: 0.4; } 50% { transform: translate(-20px,14px); opacity: 0.65; } }
    #abo1 { animation: ab-orb1 9s ease-in-out infinite; }
    #abo2 { animation: ab-orb2 11s ease-in-out infinite 1.5s; }
  `}</style>

  <svg width="860" height="210" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="abg1" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(236,72,153,0.32)" />
        <stop offset="100%" stopColor="rgba(236,72,153,0)" />
      </radialGradient>
      <radialGradient id="abg2" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(139,92,246,0.32)" />
        <stop offset="100%" stopColor="rgba(139,92,246,0)" />
      </radialGradient>
    </defs>
    <ellipse id="abo1" cx="70" cy="180" rx="200" ry="150" fill="url(#abg1)" />
    <ellipse id="abo2" cx="790" cy="40" rx="190" ry="150" fill="url(#abg2)" />
  </svg>

  <div style={{
    position: 'relative', display: 'flex', flexDirection: 'column',
    justifyContent: 'center', padding: '0 48px', zIndex: 10, gap: 12, flex: 1
  }}>
    <span style={{
      fontSize: 11, letterSpacing: 4, textTransform: 'uppercase',
      color: 'rgba(147,197,253,0.75)', fontWeight: 700
    }}>About</span>

    <span style={{ fontSize: 21, fontWeight: 700, color: '#ffffff', lineHeight: 1.35 }}>
      I design intuitive interfaces, then build them into working products.
    </span>

    <span style={{ fontSize: 14, color: 'rgba(225,222,245,0.72)', lineHeight: 1.6, maxWidth: 720 }}>
      Informatics student at UPN "Veteran" Yogyakarta. My main focus is UI/UX Design — for products in health, education, and social impact — and I also build what I design, from mobile apps to cloud-deployed systems.
    </span>

    <span style={{ fontSize: 13, color: 'rgba(196,181,253,0.65)', fontWeight: 500, marginTop: 4 }}>
      Head of UI/UX Design @ IT Club UPNVYK · UX Mentor for GEMASTIK & national design competitions
    </span>
  </div>
</div>
```

```aura width=860 height=390
<div style={{
  width: '100%', height: '100%', background: '#0a0a12',
  display: 'flex', flexDirection: 'column', alignItems: 'center',
  fontFamily: 'Inter, sans-serif', position: 'relative', overflow: 'hidden',
  borderRadius: 20, border: '1px solid rgba(236,72,153,0.14)', padding: '24px 0'
}}>

  <style>{`
    @keyframes ac-orb1 { 0%, 100% { transform: translate(0,0); opacity: 0.4; } 50% { transform: translate(30px,-20px); opacity: 0.65; } }
    @keyframes ac-orb2 { 0%, 100% { transform: translate(0,0); opacity: 0.35; } 50% { transform: translate(-25px,18px); opacity: 0.6; } }
    #aco1 { animation: ac-orb1 10s ease-in-out infinite; }
    #aco2 { animation: ac-orb2 12s ease-in-out infinite 1s; }
  `}</style>

  <svg width="860" height="390" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="acg1" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(236,72,153,0.22)" />
        <stop offset="100%" stopColor="rgba(236,72,153,0)" />
      </radialGradient>
      <radialGradient id="acg2" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(139,92,246,0.22)" />
        <stop offset="100%" stopColor="rgba(139,92,246,0)" />
      </radialGradient>
    </defs>
    <ellipse id="aco1" cx="90" cy="340" rx="220" ry="170" fill="url(#acg1)" />
    <ellipse id="aco2" cx="770" cy="40" rx="200" ry="160" fill="url(#acg2)" />
  </svg>

  <span style={{ display:'flex', fontSize:11, fontWeight:700, letterSpacing:4, textTransform:'uppercase',
    color:'rgba(249,168,212,0.75)', marginBottom:18, zIndex:10 }}>Notable Achievements</span>

  <div style={{ display:'flex', flexDirection:'column', gap:9, zIndex:10, width:'100%', padding:'0 32px' }}>
    {[
      { badge: '🥇', place: '1st Winner', desc: 'HackfestUC International UI/UX Competition', color: '236,72,153' },
      { badge: '🥇', place: '1st Winner', desc: 'Proto-A-Thon International Design Competition @BINUS · 100+ teams, 10 countries', color: '236,72,153' },
      { badge: '🥉', place: '3rd Winner', desc: 'UX Design @ GEMASTIK XVIII 2025 · 430+ teams, 100+ universities', color: '139,92,246' },
      { badge: '🥉', place: '3rd Winner', desc: 'Hackathon ElevAIte Indonesia Hub UGM · 400+ teams', color: '139,92,246' },
      { badge: '🏅', place: 'Top 9 Finalist', desc: 'UXVidia @ Arkavidia 9.0 ITB', color: '96,165,250' },
    ].map(function(item, i) {
      return (
        <div key={i} style={{
          display: 'flex', alignItems: 'center', padding: '13px 20px',
          background: 'rgba(255,255,255,0.025)',
          border: '1px solid rgba(' + item.color + ',0.20)',
          borderRadius: 12, gap: 14
        }}>
          <span style={{ display: 'flex', fontSize: 18 }}>{item.badge}</span>
          <span style={{ display: 'flex', fontSize: 14, fontWeight: 700, color: '#ffffff', flexShrink: 0, width: 118 }}>
            {item.place}
          </span>
          <span style={{ display: 'flex', fontSize: 13, color: 'rgba(225,222,245,0.68)', lineHeight: 1.4 }}>
            {item.desc}
          </span>
        </div>
      );
    })}
  </div>
</div>
```

```aura width=860 height=420
<div style={{
  width: '100%', height: '100%', background: '#0a0a12',
  display: 'flex', flexDirection: 'column', alignItems: 'center',
  fontFamily: 'Inter, sans-serif', position: 'relative', overflow: 'hidden',
  borderRadius: 20, border: '1px solid rgba(96,165,250,0.14)', padding: '24px 0'
}}>

  <style>{`
    @keyframes pj-orb1 { 0%, 100% { transform: translate(0,0); opacity: 0.35; } 50% { transform: translate(35px,-25px); opacity: 0.6; } }
    @keyframes pj-orb2 { 0%, 100% { transform: translate(0,0); opacity: 0.3; } 50% { transform: translate(-30px,20px); opacity: 0.55; } }
    #pjo1 { animation: pj-orb1 10s ease-in-out infinite; }
    #pjo2 { animation: pj-orb2 13s ease-in-out infinite 1s; }
  `}</style>

  <svg width="860" height="420" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="pjg1" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(96,165,250,0.22)" />
        <stop offset="100%" stopColor="rgba(96,165,250,0)" />
      </radialGradient>
      <radialGradient id="pjg2" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(139,92,246,0.22)" />
        <stop offset="100%" stopColor="rgba(139,92,246,0)" />
      </radialGradient>
    </defs>
    <ellipse id="pjo1" cx="100" cy="380" rx="220" ry="180" fill="url(#pjg1)" />
    <ellipse id="pjo2" cx="760" cy="40" rx="200" ry="160" fill="url(#pjg2)" />
  </svg>

  <span style={{ display:'flex', fontSize:11, fontWeight:700, letterSpacing:4, textTransform:'uppercase',
    color:'rgba(147,197,253,0.75)', marginBottom:18, zIndex:10 }}>Featured Projects</span>

  <div style={{ display: 'flex', flexDirection: 'column', gap: 10, zIndex: 10, width: '100%', padding: '0 28px' }}>
    {[
      { title: 'Sipupuk — Cloud Distribution System', desc: 'Subsidized fertilizer distribution platform — Auth Service, Core API, Deployment', tech: 'Node.js · GCP · MySQL', color: '96,165,250' },
      { title: 'LoveLock — Encryption App', desc: 'Encrypted messaging app: Scrypt, AES, ChaCha20, LSB steganography', tech: 'Python · Streamlit', color: '236,72,153' },
      { title: 'Student Performance Clustering', desc: 'K-Means/K-Medoids clustering analysis to guide academic intervention', tech: 'Python · Scikit-learn', color: '139,92,246' },
      { title: 'Grafika Komputer — Paint Tool', desc: '2D geometric transformation paint tool (translation, scale, rotation, shear)', tech: 'Python · Tkinter', color: '167,139,250' },
    ].map(function(project, i) {
      return (
        <div key={i} style={{
          display: 'flex', alignItems: 'center', padding: '15px 22px',
          background: 'rgba(255,255,255,0.025)',
          border: '1px solid rgba(' + project.color + ',0.20)',
          borderRadius: 12, gap: 16
        }}>
          <div style={{
            width: 9, height: 9, borderRadius: 5, flexShrink: 0,
            background: 'rgba(' + project.color + ',0.9)',
            boxShadow: '0 0 10px rgba(' + project.color + ',0.5)'
          }} />
          <div style={{ display: 'flex', flexDirection: 'column', gap: 4, flex: 1 }}>
            <span style={{ display: 'flex', fontSize: 15, fontWeight: 700, color: '#ffffff' }}>
              {project.title}
            </span>
            <span style={{ display: 'flex', fontSize: 12, color: 'rgba(225,222,245,0.62)', lineHeight: 1.4 }}>
              {project.desc}
            </span>
          </div>
          <span style={{
            display: 'flex', fontSize: 11, color: 'rgba(' + project.color + ',0.85)',
            fontWeight: 600, letterSpacing: 0.2, textAlign: 'right', flexShrink: 0, maxWidth: 160
          }}>{project.tech}</span>
        </div>
      );
    })}
  </div>
</div>
```

<div align="center"><sub><a href="https://github.com/mruhulj?tab=repositories">View all repositories →</a></sub></div>

```aura width=860 height=90
<div style={{
  width: '100%', height: '100%', background: '#0a0a12',
  display: 'flex', flexDirection: 'column', alignItems: 'center', justifyContent: 'center',
  fontFamily: 'Inter, sans-serif', position: 'relative', overflow: 'hidden',
  borderRadius: 20, border: '1px solid rgba(168,85,247,0.10)'
}}>

  <svg width="860" height="90" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="ftg1" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(139,92,246,0.22)" />
        <stop offset="100%" stopColor="rgba(139,92,246,0)" />
      </radialGradient>
    </defs>
    <ellipse cx="430" cy="45" rx="320" ry="65" fill="url(#ftg1)" />
  </svg>

  <div style={{ display: 'flex', alignItems: 'center', gap: 8, zIndex: 10 }}>
    <div style={{ width: 5, height: 5, borderRadius: 3, background: 'rgba(236,72,153,0.7)' }} />
    <div style={{ width: 5, height: 5, borderRadius: 3, background: 'rgba(168,85,247,0.7)' }} />
    <div style={{ width: 5, height: 5, borderRadius: 3, background: 'rgba(96,165,250,0.7)' }} />
  </div>

  <span style={{
    fontSize: 12, color: 'rgba(230,225,255,0.55)', letterSpacing: 2,
    fontWeight: 500, marginTop: 10, zIndex: 10
  }}>Muhammad Ruhul Jadid · open to design & dev collaborations</span>
</div>
```

<br>
<p align="center"><sub>𝗉𝗈𝗐𝖾𝗋𝖾𝖽 𝖻𝗒 <a href="https://github.com/collectioneur/readme-aura">𝗋𝖾𝖺𝖽𝗆𝖾-𝖺𝗎𝗋𝖺</a></sub></p>
