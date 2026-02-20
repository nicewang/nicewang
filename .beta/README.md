<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 950 900" width="100%" height="100%">
    <defs>
        <linearGradient id="bg-grad" x1="0%" y1="0%" x2="100%" y2="100%">
            <stop offset="0%" stop-color="#E0F2FE"/>
            <stop offset="50%" stop-color="#CCFBF1"/>
            <stop offset="100%" stop-color="#DCFCE7"/>
        </linearGradient>
        <linearGradient id="text-grad" x1="0%" y1="0%" x2="100%" y2="0%">
            <stop offset="0%" stop-color="#0284C7"/>
            <stop offset="100%" stop-color="#059669"/>
        </linearGradient>
        <linearGradient id="avatar-grad" x1="0%" y1="0%" x2="100%" y2="100%">
            <stop offset="0%" stop-color="#38BDF8"/>
            <stop offset="100%" stop-color="#4ADE80"/>
        </linearGradient>
        <filter id="glow" x="-20%" y="-20%" width="140%" height="140%">
            <feGaussianBlur stdDeviation="45" result="blur" />
            <feComposite in="SourceGraphic" in2="blur" operator="over" />
        </filter>
        <style>
            :root {
                --text-main: #1E293B; /* Dark slate for high contrast on light bg */
                --text-muted: #475569;
                --text-dim: #64748B;
                --accent-blue: #0284C7;
                --accent-teal: #0D9488;
                --accent-green: #059669;
                --font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;
                --font-mono: 'SFMono-Regular', Consolas, 'Liberation Mono', Menlo, monospace;
            }
            text {
                font-family: var(--font-family);
                fill: var(--text-main);
            }
            a { cursor: pointer; }
            a:hover .link-text { fill: #0369A1; text-decoration: underline; }
            .title-hi { font-size: 28px; font-weight: 800; fill: url(#text-grad); }
            .quote { font-size: 15px; font-style: italic; fill: var(--text-muted); text-anchor: middle; }
            .section-title { font-size: 18px; font-weight: 700; fill: var(--text-main); }
            .bullet { font-size: 14.5px; fill: var(--text-muted); }
            .sub-bullet { font-size: 14px; fill: var(--text-dim); }
            .bold-text { font-weight: 700; fill: var(--text-main); }
            .small-text { font-size: 12.5px; fill: var(--text-dim); }
            .link-text { fill: var(--accent-blue); font-weight: 600; text-decoration: underline; transition: fill 0.3s; }
            .code-text { fill: var(--accent-teal); font-family: var(--font-mono); font-size: 13.5px; }
            .tag-bg { fill: #F0FDF4; stroke: #A7F3D0; stroke-width: 1.5; }
            .tag-text { font-size: 12.5px; font-weight: 600; fill: var(--accent-green); text-anchor: middle; }
            @keyframes fadeIn {
                0% { opacity: 0; transform: translateY(15px); }
                100% { opacity: 1; transform: translateY(0); }
            }
            @keyframes wave {
                0%, 100% { transform: rotate(0deg); }
                25% { transform: rotate(-20deg); }
                75% { transform: rotate(20deg); }
            }
            @keyframes float {
                0%, 100% { transform: translateY(0); }
                50% { transform: translateY(-15px); }
            }
            .fade-in { animation: fadeIn 1s ease-out forwards; opacity: 0; }
            .delay-1 { animation-delay: 0.1s; }
            .delay-2 { animation-delay: 0.3s; }
            .delay-3 { animation-delay: 0.5s; }
            .delay-4 { animation-delay: 0.7s; }
            .delay-5 { animation-delay: 0.9s; }
            .delay-6 { animation-delay: 1.1s; }
            .wave-hand { 
                display: inline-block; 
                transform-origin: 70% 70%; 
                animation: wave 2s infinite; 
            }
            .floating { animation: float 6s ease-in-out infinite; }
            .floating-alt { animation: float 8s ease-in-out infinite alternate-reverse; }
        </style>
    </defs>
    <rect width="100%" height="100%" fill="url(#bg-grad)" rx="16" />
    <circle cx="850" cy="200" r="160" fill="#7DD3FC" filter="url(#glow)" opacity="0.4" class="floating" />
    <circle cx="100" cy="700" r="200" fill="#86EFAC" filter="url(#glow)" opacity="0.4" class="floating-alt" />
    <circle cx="500" cy="50" r="120" fill="#6EE7B7" filter="url(#glow)" opacity="0.35" class="floating" />
    <g transform="translate(50, 50)">
        <g transform="translate(0, 0)">
            <g class="fade-in delay-1">
                <text x="0" y="20" class="title-hi">Hi there <tspan class="wave-hand">👋</tspan></text>
                <text x="425" y="65" class="quote">"The <tspan class="bold-text">trade-off</tspan> is the key word in my life, and do the <tspan class="bold-text">indeed</tspan> work~"</text>
            </g>
        </g>
        <g transform="translate(750, 10)">
            <g class="fade-in delay-2">
                <g class="floating">
                    <circle cx="0" cy="0" r="55" fill="url(#avatar-grad)" />
                    <text x="0" y="12" font-size="32" font-weight="bold" fill="#ffffff" text-anchor="middle">XW</text>
                    <circle cx="35" cy="35" r="14" fill="#FFFFFF" stroke="#E2E8F0" stroke-width="3"/>
                    <text x="35" y="40" font-size="14" text-anchor="middle">👩🏻‍💻</text>
                </g>
            </g>
        </g>
        <g transform="translate(0, 120)">
            <g class="fade-in delay-2">
                <text x="0" y="0" class="bullet">
                    <tspan>- 🔭 I am Nice </tspan>
                    <tspan class="small-text">(Xiaonan Wang in Chinese)</tspan>
                    <tspan>, a seasoned machine learning scientist with several years industrial</tspan>
                </text>
                <text x="14" y="24" class="bullet">
                    <tspan>working experience at Chinese famous technology companies like </tspan>
                    <a href="https://www.baidu.com" target="_blank"><tspan class="link-text">Baidu</tspan></a>
                    <tspan> and </tspan>
                    <a href="https://www.antgroup.com/en" target="_blank"><tspan class="link-text">Ant Group</tspan></a>
                    <tspan>.</tspan>
                </text>
                <text x="25" y="52" class="sub-bullet">
                    <tspan>◦ Specialize in industrial applied machine learning in </tspan>
                    <tspan class="code-text">recommendation</tspan>
                    <tspan>, </tspan>
                    <tspan class="code-text">searching</tspan>
                    <tspan> and </tspan>
                    <tspan class="code-text">AdTech</tspan>
                </text>
                <text x="25" y="78" class="sub-bullet">
                    <tspan>◦ Experience in </tspan>
                    <tspan class="code-text">recall</tspan>
                    <tspan>, </tspan>
                    <tspan class="code-text">ranking</tspan>
                    <tspan>, and </tspan>
                    <tspan class="code-text">CTR prediction</tspan>
                    <tspan> using </tspan>
                    <tspan class="code-text">deep learning</tspan>
                    <tspan> and </tspan>
                    <tspan class="code-text">generative AI</tspan>
                </text>
            </g>
        </g>
        <g transform="translate(0, 250)">
            <g class="fade-in delay-3">
                <text x="0" y="0" class="section-title">- 🏫 Educational Background:</text>
                <text x="25" y="32" class="bullet">
                    <tspan>◦ M.S. in Electrical Engineering at </tspan>
                    <a href="https://www.usnews.com/education/best-global-universities/university-of-electronic-science-technology-of-china-506780" target="_blank">
                        <tspan class="link-text">UESTC</tspan>
                    </a>
                </text>
                <text x="45" y="58" class="sub-bullet">
                    <tspan>📖 Master's Thesis: </tspan>
                    <a href="https://nicewang.github.io/niceproject/2023/04/18/master-thesis/" target="_blank">
                        <tspan class="link-text">Time-Sequential Wind Dancing Signal Anomaly Detection</tspan>
                    </a>
                </text>
                <text x="45" y="84" class="sub-bullet">
                    <tspan>🧐 Highlighted Research Project: </tspan>
                    <a href="https://nicewang.github.io/niceproject/2023/04/19/ship-identification/" target="_blank">
                        <tspan class="link-text">Vision-based Ship Identification</tspan>
                    </a>
                </text>
                <text x="25" y="118" class="bullet">
                    <tspan>◦ B.S. in Electrical Engineering at </tspan>
                    <a href="https://www.usnews.com/education/best-global-universities/hohai-university-528997" target="_blank">
                        <tspan class="link-text">HHU</tspan>
                    </a>
                </text>
                <text x="45" y="144" class="sub-bullet">
                    <tspan>📖 Bachelor's Thesis: </tspan>
                    <a href="https://github.com/nicewang/Phased-Array-Ultrasonic-Signal-Generator" target="_blank">
                        <tspan class="link-text">Phased Array Ultrasonic Signal Generator</tspan>
                    </a>
                </text>
            </g>
        </g>
        <g transform="translate(0, 440)">
            <g class="fade-in delay-4">
                <text x="0" y="0" class="section-title">- 🌱 Current POIs (Points of Interest):</text>
                <text x="25" y="32" class="bullet">
                    <tspan>◦ 🤖️ Intersection between </tspan>
                    <tspan class="bold-text">Motion Planning</tspan>
                    <tspan>, </tspan>
                    <tspan class="bold-text">Robot Learning</tspan>
                    <tspan> and </tspan>
                    <tspan class="bold-text">Machine Learning</tspan>
                </text>
                <text x="45" y="58" class="sub-bullet">
                    <tspan>🌍 </tspan>
                    <a href="https://nicewang.github.io/niceproject/learning/robotics/" target="_blank">
                        <tspan class="link-text">Robotics Exploration &amp; Summarization &amp; Mini Presentation</tspan>
                    </a>
                </text>
                <text x="25" y="88" class="bullet">◦ Machine Learning for EE and Computer Systems</text>
                <text x="25" y="116" class="bullet">◦ Machine Learning and Artificial Intelligence</text>
            </g>
        </g>
        <g transform="translate(0, 595)">
            <g class="fade-in delay-5">
                <text x="0" y="0" class="section-title">- 👩🏻‍💻 Programming Languages &amp; ML Frameworks &amp; Big Data Technologies:</text>
                <g transform="translate(25, 20)">
                    <rect x="0" y="0" width="70" height="26" rx="13" class="tag-bg"/>
                    <text x="35" y="17.5" class="tag-text">C/C++</text>
                    <rect x="80" y="0" width="75" height="26" rx="13" class="tag-bg"/>
                    <text x="117.5" y="17.5" class="tag-text">Python</text>
                    <rect x="165" y="0" width="60" height="26" rx="13" class="tag-bg"/>
                    <text x="195" y="17.5" class="tag-text">Java</text>
                    <rect x="235" y="0" width="115" height="26" rx="13" class="tag-bg"/>
                    <text x="292.5" y="17.5" class="tag-text">Verilog/VHDL</text>
                </g>
                <g transform="translate(25, 56)">
                    <rect x="0" y="0" width="85" height="26" rx="13" class="tag-bg"/>
                    <text x="42.5" y="17.5" class="tag-text">PyTorch</text>
                    <rect x="95" y="0" width="105" height="26" rx="13" class="tag-bg"/>
                    <text x="147.5" y="17.5" class="tag-text">TensorFlow</text>
                    <rect x="210" y="0" width="65" height="26" rx="13" class="tag-bg"/>
                    <text x="242.5" y="17.5" class="tag-text">Keras</text>
                </g>
                <g transform="translate(25, 92)">
                    <rect x="0" y="0" width="165" height="26" rx="13" class="tag-bg"/>
                    <text x="82.5" y="17.5" class="tag-text">Hadoop/Map-Reduce</text>
                    <rect x="175" y="0" width="85" height="26" rx="13" class="tag-bg"/>
                    <text x="217.5" y="17.5" class="tag-text">PySpark</text>
                </g>
            </g>
        </g>
        <g transform="translate(0, 755)">
            <g class="fade-in delay-6">
                <text x="0" y="0" class="section-title">- 🔗 Quick Links:</text>
                <text x="25" y="30" class="bullet">
                    <tspan>◦ </tspan>
                    <a href="https://nicewang.github.io/niceproject/" target="_blank">
                        <tspan class="link-text">NiceWang's Projects: Highlighted Projects' Page</tspan>
                    </a>
                </text>
                <text x="25" y="58" class="bullet">
                    <tspan>◦ </tspan>
                    <a href="https://www.youtube.com/@XiaonanNiceWang" target="_blank">
                        <tspan class="link-text">YouTube Channel</tspan>
                    </a>
                </text>
                <text x="25" y="86" class="bullet">
                    <tspan>◦ </tspan>
                    <a href="https://scholar.google.com/citations?user=ipnvcRoAAAAJ&amp;hl" target="_blank">
                        <tspan class="link-text">Google Scholar</tspan>
                    </a>
                </text>
            </g>
        </g>    
    </g>
</svg>