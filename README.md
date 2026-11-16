<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 800 400" width="800" height="400" xmlns:c2pa="http://c2pa.org/manifest">
  <defs>
    <linearGradient id="bg" x1="0" y1="0" x2="0" y2="1">
      <stop offset="0" stop-color="#0d0221"/>
      <stop offset="0.6" stop-color="#2a0a4a"/>
      <stop offset="1" stop-color="#4a0a5c"/>
    </linearGradient>
    <linearGradient id="sun" x1="0" y1="0" x2="0" y2="1">
      <stop offset="0" stop-color="#fcee0a"/>
      <stop offset="1" stop-color="#ff00cc"/>
    </linearGradient>
    <linearGradient id="floor" x1="0" y1="0" x2="0" y2="1">
      <stop offset="0" stop-color="#1a0b3d"/>
      <stop offset="1" stop-color="#07010f"/>
    </linearGradient>
    <filter id="glow" x="-50%" y="-50%" width="200%" height="200%">
      <feGaussianBlur stdDeviation="4" result="b"/>
      <feMerge><feMergeNode in="b"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <filter id="blur"><feGaussianBlur stdDeviation="14"/></filter>
    <clipPath id="screen"><rect x="528" y="208" width="184" height="94" rx="3"/></clipPath>
    <pattern id="scan" width="4" height="4" patternUnits="userSpaceOnUse">
      <rect width="4" height="1" fill="#000" opacity="0.25"/>
    </pattern>
    <g id="code">
      <rect x="0" y="0" width="60" height="5" rx="2" fill="#ff00cc"/><rect x="70" y="0" width="40" height="5" rx="2" fill="#00e5ff"/>
      <rect x="12" y="14" width="90" height="5" rx="2" fill="#00e5ff"/>
      <rect x="12" y="28" width="50" height="5" rx="2" fill="#a974ff"/><rect x="68" y="28" width="70" height="5" rx="2" fill="#ff00cc"/>
      <rect x="24" y="42" width="100" height="5" rx="2" fill="#00e5ff"/>
      <rect x="24" y="56" width="40" height="5" rx="2" fill="#fcee0a"/><rect x="70" y="56" width="60" height="5" rx="2" fill="#a974ff"/>
      <rect x="12" y="70" width="80" height="5" rx="2" fill="#ff00cc"/>
      <rect x="0" y="84" width="30" height="5" rx="2" fill="#00e5ff"/><rect x="40" y="84" width="90" height="5" rx="2" fill="#a974ff"/>
      <rect x="12" y="98" width="55" height="5" rx="2" fill="#fcee0a"/><rect x="75" y="98" width="45" height="5" rx="2" fill="#00e5ff"/>
    </g>
  </defs>
  <style>
    .scroll{animation:scroll 6s linear infinite}
    @keyframes scroll{from{transform:translateY(0)}to{transform:translateY(-112px)}}
    .rain{stroke:#00e5ff;stroke-width:1;opacity:.35;animation:fall 1.4s linear infinite}
    @keyframes fall{from{transform:translateY(-60px)}to{transform:translateY(440px)}}
    .blink{animation:blink 3s steps(1) infinite}
    @keyframes blink{0%,45%{opacity:1}50%,60%{opacity:.1}65%,100%{opacity:1}}
    .flicker{animation:flicker 4s infinite}
    @keyframes flicker{0%,18%,22%,62%,64%,100%{opacity:1}20%,63%{opacity:.35}}
    .cursor{animation:cur 1s steps(1) infinite}
    @keyframes cur{0%,50%{opacity:1}51%,100%{opacity:0}}
    .pulse{animation:pulse 2.5s ease-in-out infinite}
    @keyframes pulse{0%,100%{opacity:.25}50%{opacity:.5}}
    text{font-family:'Courier New',monospace}
  </style>

  <!-- sky -->
  <rect width="800" height="400" fill="url(#bg)"/>
  <circle cx="400" cy="175" r="85" fill="url(#sun)" opacity="0.9"/>
  <rect x="310" y="190" width="180" height="3" fill="#2a0a4a"/>
  <rect x="310" y="205" width="180" height="4" fill="#2a0a4a"/>
  <rect x="310" y="222" width="180" height="5" fill="#2a0a4a"/>

  <!-- skyline -->
  <g fill="#120a2e">
    <rect x="0" y="210" width="60" height="130"/><rect x="60" y="170" width="45" height="170"/>
    <rect x="105" y="230" width="70" height="110"/><rect x="175" y="150" width="50" height="190"/>
    <rect x="225" y="215" width="60" height="125"/><rect x="285" y="245" width="70" height="95"/>
    <rect x="450" y="235" width="60" height="105"/><rect x="510" y="160" width="55" height="180"/>
    <rect x="565" y="225" width="70" height="115"/><rect x="635" y="140" width="50" height="200"/>
    <rect x="685" y="205" width="55" height="135"/><rect x="740" y="180" width="60" height="160"/>
  </g>
  <g fill="#00e5ff" opacity="0.8">
    <rect class="blink" x="70" y="185" width="5" height="5"/><rect x="85" y="205" width="5" height="5"/>
    <rect x="185" y="170" width="5" height="5"/><rect class="blink" x="200" y="195" width="5" height="5" style="animation-delay:1s"/>
    <rect x="520" y="180" width="5" height="5"/><rect class="blink" x="540" y="210" width="5" height="5" style="animation-delay:2s"/>
    <rect x="645" y="160" width="5" height="5"/><rect x="660" y="185" width="5" height="5"/>
    <rect class="blink" x="750" y="200" width="5" height="5" style="animation-delay:.5s"/>
  </g>
  <g fill="#ff00cc" opacity="0.8">
    <rect x="15" y="230" width="5" height="5"/><rect class="blink" x="30" y="255" width="5" height="5" style="animation-delay:1.5s"/>
    <rect x="120" y="250" width="5" height="5"/><rect x="235" y="235" width="5" height="5"/>
    <rect class="blink" x="460" y="255" width="5" height="5" style="animation-delay:2.4s"/><rect x="580" y="245" width="5" height="5"/>
    <rect x="700" y="225" width="5" height="5"/><rect x="760" y="205" width="5" height="5"/>
  </g>

  <!-- title -->
  <text x="24" y="40" font-size="18" fill="#00e5ff" filter="url(#glow)" class="flicker">&gt; SYSTEM.ONLINE<tspan class="cursor">_</tspan></text>
  <text x="24" y="62" font-size="12" fill="#ff00cc">// dev.mode = ACTIVE</text>
  <text x="776" y="40" font-size="14" fill="#fcee0a" text-anchor="end" filter="url(#glow)" class="flicker" style="animation-delay:1.2s">JAVA · AI · ROBOTICS</text>

  <!-- floor -->
  <rect x="0" y="340" width="800" height="60" fill="url(#floor)"/>
  <rect x="0" y="340" width="800" height="2" fill="#ff00cc" filter="url(#glow)" opacity="0.8"/>

  <!-- monitor glow -->
  <rect x="500" y="190" width="240" height="140" fill="#00e5ff" opacity="0.35" filter="url(#blur)" class="pulse"/>

  <!-- desk -->
  <rect x="430" y="330" width="340" height="10" rx="2" fill="#1a0f3d" stroke="#ff00cc" stroke-width="1.5"/>
  <rect x="450" y="340" width="8" height="55" fill="#120a2e"/><rect x="742" y="340" width="8" height="55" fill="#120a2e"/>

  <!-- monitor -->
  <rect x="616" y="312" width="12" height="18" fill="#120a2e"/>
  <rect x="590" y="326" width="64" height="4" rx="2" fill="#120a2e"/>
  <rect x="520" y="200" width="200" height="112" rx="6" fill="#050110" stroke="#00e5ff" stroke-width="2" filter="url(#glow)"/>
  <rect x="528" y="208" width="184" height="94" rx="3" fill="#07031a"/>
  <g clip-path="url(#screen)">
    <g class="scroll">
      <use href="#code" x="536" y="212"/>
      <use href="#code" x="536" y="324"/>
    </g>
  </g>
  <rect x="528" y="208" width="184" height="94" rx="3" fill="url(#scan)"/>

  <!-- keyboard -->
  <rect x="446" y="322" width="70" height="7" rx="2" fill="#0b0620" stroke="#ff00cc" stroke-width="1" filter="url(#glow)"/>

  <!-- chair -->
  <rect x="262" y="262" width="14" height="72" rx="7" fill="#1a0f3d" stroke="#ff00cc" stroke-width="1.5"/>
  <rect x="268" y="328" width="130" height="10" rx="5" fill="#1a0f3d" stroke="#ff00cc" stroke-width="1.5"/>
  <rect x="325" y="338" width="8" height="40" fill="#120a2e"/>
  <rect x="295" y="376" width="70" height="6" rx="3" fill="#120a2e"/>

  <!-- man -->
  <g>
    <!-- legs -->
    <path d="M296 322 H424 V344 H296 Z" fill="#0b0620"/>
    <rect x="410" y="342" width="18" height="46" rx="4" fill="#0b0620"/>
    <rect x="404" y="384" width="34" height="9" rx="4" fill="#ff00cc"/>
    <!-- torso / hoodie -->
    <path d="M280 330 L286 268 Q330 232 378 268 L392 330 Z" fill="#150a33"/>
    <path d="M378 268 L392 330" stroke="#00e5ff" stroke-width="2" opacity="0.8" filter="url(#glow)"/>
    <!-- arm -->
    <path d="M370 280 L420 312 L452 322" stroke="#150a33" stroke-width="14" stroke-linecap="round" stroke-linejoin="round" fill="none"/>
    <path d="M420 312 L452 322" stroke="#00e5ff" stroke-width="2" opacity="0.7" fill="none"/>
    <!-- head + hood -->
    <circle cx="336" cy="232" r="27" fill="#150a33"/>
    <path d="M309 232 Q310 202 340 204 Q364 206 362 232 Q350 214 328 218 Q312 222 309 232 Z" fill="#0b0620"/>
    <path d="M362 226 Q364 240 356 252" stroke="#00e5ff" stroke-width="2" fill="none" opacity="0.9" filter="url(#glow)"/>
    <!-- headphones -->
    <path d="M311 232 Q312 196 338 196 Q362 197 362 228" stroke="#ff00cc" stroke-width="5" fill="none" filter="url(#glow)"/>
    <rect x="306" y="226" width="10" height="20" rx="4" fill="#ff00cc"/>
    <rect x="356" y="224" width="10" height="20" rx="4" fill="#00e5ff"/>
    <!-- visor -->
    <rect x="352" y="228" width="16" height="5" rx="2" fill="#00e5ff" filter="url(#glow)" class="pulse" style="opacity:.9"/>
  </g>

  <!-- rain -->
  <g>
    <line class="rain" x1="30" y1="0" x2="26" y2="18" style="animation-delay:0s"/>
    <line class="rain" x1="90" y1="0" x2="86" y2="18" style="animation-delay:.3s"/>
    <line class="rain" x1="150" y1="0" x2="146" y2="18" style="animation-delay:.8s"/>
    <line class="rain" x1="210" y1="0" x2="206" y2="18" style="animation-delay:.1s"/>
    <line class="rain" x1="270" y1="0" x2="266" y2="18" style="animation-delay:1s"/>
    <line class="rain" x1="330" y1="0" x2="326" y2="18" style="animation-delay:.5s"/>
    <line class="rain" x1="390" y1="0" x2="386" y2="18" style="animation-delay:1.2s"/>
    <line class="rain" x1="450" y1="0" x2="446" y2="18" style="animation-delay:.2s"/>
    <line class="rain" x1="510" y1="0" x2="506" y2="18" style="animation-delay:.9s"/>
    <line class="rain" x1="570" y1="0" x2="566" y2="18" style="animation-delay:.6s"/>
    <line class="rain" x1="630" y1="0" x2="626" y2="18" style="animation-delay:1.1s"/>
    <line class="rain" x1="690" y1="0" x2="686" y2="18" style="animation-delay:.4s"/>
    <line class="rain" x1="750" y1="0" x2="746" y2="18" style="animation-delay:.7s"/>
    <line class="rain" x1="60" y1="0" x2="56" y2="18" style="animation-delay:1.3s"/>
    <line class="rain" x1="480" y1="0" x2="476" y2="18" style="animation-delay:.15s"/>
    <line class="rain" x1="720" y1="0" x2="716" y2="18" style="animation-delay:.95s"/>
  </g>

  <!-- scanlines + border -->
  <rect width="800" height="400" fill="url(#scan)" opacity="0.5"/>
  <rect x="1" y="1" width="798" height="398" fill="none" stroke="#ff00cc" stroke-width="2" opacity="0.6"/>
<metadata><c2pa:manifest>AAAWgmp1bWIAAAAeanVtZGMycGEAEQAQgAAAqgA4m3EDYzJwYQAAABZcanVtYgAAAEdqdW1kYzJtYQARABCAAACqADibcQN1cm46YzJwYToyYjY0ZjhjNy05ZjE5LTQyNjQtYmU2ZS02MDkzNWZmNWY5MTAAAAADl2p1bWIAAAApanVtZGMyYXMAEQAQgAAAqgA4m3EDYzJwYS5hc3NlcnRpb25zAAAAALxqdW1iAAAARGp1bWRjYm9yABEAEIAAAKoAOJtxE2MycGEuaW5ncmVkaWVudC52MwAAAAAYYzJzaGJS1rzay/zQidcfGhEUZPkAAABwY2JvcqNpZGM6Zm9ybWF0bWltYWdlL3N2Zyt4bWxqaW5zdGFuY2VJRHgseG1wOmlpZDo3NGIwNWYzNS1lZWY3LTQyMmYtOTY3My02NTY5ZjgyMWM2ODhscmVsYXRpb25zaGlwaHBhcmVudE9mAAAB4mp1bWIAAABBanVtZGNib3IAEQAQgAAAqgA4m3ETYzJwYS5hY3Rpb25zLnYyAAAAABhjMnNotzeZ180l3JVolLe3qjBt/AAAAZljYm9yomdhY3Rpb25zgqJmYWN0aW9ua2MycGEub3BlbmVkanBhcmFtZXRlcnOha2luZ3JlZGllbnRzgaJjdXJseC1zZWxmI2p1bWJmPWMycGEuYXNzZXJ0aW9ucy9jMnBhLmluZ3JlZGllbnQudjNkaGFzaFgg3Pm7/idk3pllDBxmaa86axXbdAjpDd5GgUNkqkcoq2ikZmFjdGlvbngdY29tLmFudGhyb3BpYy5jbGF1ZGUucHJvdmlkZWRqcGFyYW1ldGVyc6F4H2NvbS5hbnRocm9waWMub3JpZ2luLWNvbmZpZGVuY2VndW5rbm93bmtkZXNjcmlwdGlvbnhmQ2xhdWRlIHByb3ZpZGVkIHRoaXMgZmlsZSBhdCB0aGUgcmVxdWVzdCBvZiBhIHVzZXIgYW5kIG1heSBoYXZlIGNyZWF0ZWQgb3IgbW9kaWZpZWQgdGhlIGZpbGUgY29udGVudHMubXNvZnR3YXJlQWdlbnShZG5hbWVmQ2xhdWRlcmFsbEFjdGlvbnNJbmNsdWRlZPUAAADIanVtYgAAAEBqdW1kY2JvcgARABCAAACqADibcRNjMnBhLmhhc2guZGF0YQAAAAAYYzJzaOGPt0VLXCUj6fCvW0BFa8YAAACAY2JvcqVjYWxnZnNoYTI1NmNwYWRMAAAAAAAAAAAAAAAAZGhhc2hYIAzZluIerWONDWVwYaxDRCP9Yqb7WuQidRIt+VeNm9eKZG5hbWVuanVtYmYgbWFuaWZlc3RqZXhjbHVzaW9uc4GiZXN0YXJ0GSfvZmxlbmd0aBkeBAAAAj5qdW1iAAAAJ2p1bWRjMmNsABEAEIAAAKoAOJtxA2MycGEuY2xhaW0udjIAAAACD2Nib3KlY2FsZ2ZzaGEyNTZpc2lnbmF0dXJleE1zZWxmI2p1bWJmPS9jMnBhL3VybjpjMnBhOjJiNjRmOGM3LTlmMTktNDI2NC1iZTZlLTYwOTM1ZmY1ZjkxMC9jMnBhLnNpZ25hdHVyZWppbnN0YW5jZUlEeCx4bXA6aWlkOjFjM2I5ODMwLTcyMTctNDI4Ni1hOTYwLTZlZjcxMGE3YjM0MnJjcmVhdGVkX2Fzc2VydGlvbnODomN1cmx4LXNlbGYjanVtYmY9YzJwYS5hc3NlcnRpb25zL2MycGEuaW5ncmVkaWVudC52M2RoYXNoWCDc+bv+J2TemWUMHGZprzprFdt0COkN3kaBQ2SqRyiraKJjdXJseCpzZWxmI2p1bWJmPWMycGEuYXNzZXJ0aW9ucy9jMnBhLmFjdGlvbnMudjJkaGFzaFggZkMR4oJ2z6dhLN4obXHNQjCvHNV1xrpy10tiOVh1TT2iY3VybHgpc2VsZiNqdW1iZj1jMnBhLmFzc2VydGlvbnMvYzJwYS5oYXNoLmRhdGFkaGFzaFggXjPgnDdaGZ/KO7l2zLuB3P4sTDNO/knZ5QyUrid+B+N0Y2xhaW1fZ2VuZXJhdG9yX2luZm+jZG5hbWVvQW50aHJvcGljIEZpbGVzZ3ZlcnNpb25lMS4wLjBrc3BlY1ZlcnNpb25lMi40LjAAABA4anVtYgAAAChqdW1kYzJjcwARABCAAACqADibcQNjMnBhLnNpZ25hdHVyZQAAABAIY2JvctKEWQISogEmGCFZAgowggIGMIIBjaADAgECAhRA5aAK7sI50L64g/oGQgU9Z1UTADAKBggqhkjOPQQDAzBJMRcwFQYDVQQKEw5BbnRocm9waWMsIFBCQzEuMCwGA1UEAxMlQW50aHJvcGljIENvbnRlbnQgQ3JlZGVudGlhbHMgUm9vdCBDQTAeFw0yNjA4MDcxODQzNTZaFw0yODA4MDYxOTQzNTZaMEQxFzAVBgNVBAoTDkFudGhyb3BpYywgUEJDMSkwJwYDVQQDEyBBbnRocm9waWMgQ2xhdWRlIENvbnRlbnQgU2lnbmluZzBZMBMGByqGSM49AgEGCCqGSM49AwEHA0IABJh6CmvLUBgFFNU0vUKlOVtE6djd17L5SuwX0LemFisBM3dkd/3cyjxFA3Qo5S46fX0/ihY0VZ7mfb9KF703t5OjWDBWMA4GA1UdDwEB/wQEAwIHgDAVBgNVHSUEDjAMBgorBgEEAYPoXgIBMAwGA1UdEwEB/wQCMAAwHwYDVR0jBBgwFoAUzlHiBIFOZFsj+OPEz5o+nMHXXMIwCgYIKoZIzj0EAwMDZwAwZAIwMXMdFJ4BetLLVY7ORuE9noqbbAZOZn/aArXyTwFAZfKrPzxF2vPoJNf1+UCdg1XGAjBwX1zd9WGqYkqmL5SFqw1QySjr1zJfpJM9+1rdDwSPLMOPOjKuiXjoU/pUUeG9RwmhY3BhZFkNngAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAPZYQN1Lkvl53yqgeXZqvqOh6Kh1bIYOyZIyKK3zu3mN6crD0aaEGL8BW+3mUjHSp0wuqJlpfo9+hBuSxV0xJb1CIY0=</c2pa:manifest></metadata></svg>
