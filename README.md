# PRODIGY_Wb_04
task 04 of my internship on web development at infotech
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Alex Johnson - Web Developer Portfolio</title>
    <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.2.19/dist/tailwind.min.css" rel="stylesheet">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@fortawesome/fontawesome-free@6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Poppins', sans-serif;
        }
        .gradient-bg {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
        }
        .card-hover {
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        .card-hover:hover {
            transform: translateY(-5px);
            box-shadow: 0 20px 40px rgba(0,0,0,0.1);
        }
        .skill-bar {
            height: 8px;
            background: linear-gradient(90deg, #667eea, #764ba2);
            border-radius: 4px;
            transition: width 1s ease;
        }
        .professional-photo {
            width: 200px;
            height: 200px;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 4rem;
            margin: 0 auto;
        }
        .project-image {
            width: 100%;
            height: 200px;
            background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);
            border-radius: 8px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 2rem;
        }
        .timeline-item::before {
            content: '';
            position: absolute;
            left: 0;
            top: 0;
            width: 4px;
            height: 100%;
            background: linear-gradient(135deg, #667eea, #764ba2);
            border-radius: 2px;
        }
    </style>
</head>
<body class="bg-gray-50">
    <!-- Navigation -->
    <nav class="fixed top-0 w-full bg-white shadow-md z-50">
        <div class="container mx-auto px-6 py-4">
            <div class="flex justify-between items-center">
                <div class="text-2xl font-bold text-gray-800">Alex Johnson</div>
                <div class="hidden md:flex space-x-8">
                    <a href="#home" class="text-gray-600 hover:text-purple-600 transition">Home</a>
                    <a href="#about" class="text-gray-600 hover:text-purple-600 transition">About</a>
                    <a href="#skills" class="text-gray-600 hover:text-purple-600 transition">Skills</a>
                    <a href="#projects" class="text-gray-600 hover:text-purple-600 transition">Projects</a>
                    <a href="#contact" class="text-gray-600 hover:text-purple-600 transition">Contact</a>
                </div>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="gradient-bg text-white py-24 mt-16">
        <div class="container mx-auto px-6 text-center">
            <div class="professional-photo mb-8">
                <i class="fas fa-user"></i>
            </div>
            <h1 class="text-5xl md:text-6xl font-bold mb-4">Alex Johnson</h1>
            <h2 class="text-2xl md:text-3xl font-light mb-6">Full-Stack Web Developer</h2>
            <p class="text-xl mb-8 max-w-2xl mx-auto">Passionate about creating innovative web solutions that combine beautiful design with powerful functionality. Specializing in modern JavaScript frameworks and scalable backend architectures.</p>
            <div class="flex justify-center space-x-6">
                <a href="#contact" class="bg-white text-purple-600 px-8 py-3 rounded-full font-semibold hover:bg-gray-100 transition">Get In Touch</a>
                <a href="#projects" class="border-2 border-white px-8 py-3 rounded-full font-semibold hover:bg-white hover:text-purple-600 transition">View My Work</a>
            </div>
        </div>
    </section>

    <!-- About Me Section -->
    <section id="about" class="py-20">
        <div class="container mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="text-4xl font-bold text-gray-800 mb-4">About Me</h2>
                <div class="w-24 h-1 bg-gradient-to-r from-purple-500 to-blue-500 mx-auto"></div>
            </div>
            
            <div class="grid md:grid-cols-2 gap-12 items-center">
                <div>
                    <h3 class="text-2xl font-semibold mb-6 text-gray-800">My Journey</h3>
                    <p class="text-gray-600 mb-6 leading-relaxed">
                        With over 5 years of experience in web development, I've had the privilege of working with startups, established companies, and individual clients to bring their digital visions to life. My journey began with a Computer Science degree from Stanford University, where I discovered my passion for creating seamless user experiences.
                    </p>
                    <p class="text-gray-600 mb-6 leading-relaxed">
                        I specialize in full-stack development, combining my expertise in front-end technologies like React, Vue.js, and modern CSS frameworks with robust back-end solutions using Node.js, Python, and cloud services. I believe in writing clean, maintainable code and staying current with the latest industry trends and best practices.
                    </p>
                    <p class="text-gray-600 leading-relaxed">
                        When I'm not coding, you'll find me contributing to open-source projects, mentoring junior developers, or exploring new technologies that could enhance my development toolkit.
                    </p>
                </div>
                
                <div class="space-y-8">
                    <div class="bg-white rounded-lg shadow-lg p-6 card-hover">
                        <div class="flex items-center mb-4">
                            <i class="fas fa-graduation-cap text-purple-600 text-2xl mr-4"></i>
                            <h4 class="text-xl font-semibold">Education</h4>
                        </div>
                        <div class="space-y-4">
                            <div class="relative pl-6 timeline-item">
                                <h5 class="font-semibold text-gray-800">Bachelor of Science in Computer Science</h5>
                                <p class="text-purple-600 font-medium">Stanford University</p>
                                <p class="text-gray-600 text-sm">2016 - 2020 | GPA: 3.8/4.0</p>
                            </div>
                            <div class="relative pl-6 timeline-item">
                                <h5 class="font-semibold text-gray-800">Full-Stack Web Development Bootcamp</h5>
                                <p class="text-purple-600 font-medium">General Assembly</p>
                                <p class="text-gray-600 text-sm">2020 | Distinguished Graduate</p>
                            </div>
                        </div>
                    </div>
                    
                    <div class="bg-white rounded-lg shadow-lg p-6 card-hover">
                        <div class="flex items-center mb-4">
                            <i class="fas fa-briefcase text-purple-600 text-2xl mr-4"></i>
                            <h4 class="text-xl font-semibold">Professional Experience</h4>
                        </div>
                        <div class="space-y-4">
                            <div class="relative pl-6 timeline-item">
                                <h5 class="font-semibold text-gray-800">Senior Full-Stack Developer</h5>
                                <p class="text-purple-600 font-medium">TechCorp Solutions</p>
                                <p class="text-gray-600 text-sm">2022 - Present</p>
                                <p class="text-gray-600 text-sm mt-1">Leading development of scalable web applications serving 100k+ users</p>
                            </div>
                            <div class="relative pl-6 timeline-item">
                                <h5 class="font-semibold text-gray-800">Front-End Developer</h5>
                                <p class="text-purple-600 font-medium">Digital Innovations Inc.</p>
                                <p class="text-gray-600 text-sm">2020 - 2022</p>
                                <p class="text-gray-600 text-sm mt-1">Developed responsive web applications using React and modern CSS frameworks</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Skills Section -->
    <section id="skills" class="py-20 bg-white">
        <div class="container mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="text-4xl font-bold text-gray-800 mb-4">Skills & Expertise</h2>
                <div class="w-24 h-1 bg-gradient-to-r from-purple-500 to-blue-500 mx-auto"></div>
                <p class="text-gray-600 mt-4 max-w-2xl mx-auto">Here are the technologies and tools I work with to bring ideas to life</p>
            </div>
            
            <div class="grid md:grid-cols-3 gap-8">
                <!-- Frontend Skills -->
                <div class="bg-gray-50 rounded-lg p-8 card-hover">
                    <div class="text-center mb-6">
                        <i class="fas fa-code text-purple-600 text-4xl mb-4"></i>
                        <h3 class="text-xl font-semibold text-gray-800">Frontend Development</h3>
                    </div>
                    <div class="space-y-4">
                        <div>
                            <div class="flex justify-between mb-2">
                                <span class="text-gray-700">JavaScript/TypeScript</span>
                                <span class="text-gray-600">95%</span>
                            </div>
                            <div class="bg-gray-200 rounded-full h-2">
                                <div class="skill-bar" style="width: 95%"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between mb-2">
                                <span class="text-gray-700">React.js</span>
                                <span class="text-gray-600">90%</span>
                            </div>
                            <div class="bg-gray-200 rounded-full h-2">
                                <div class="skill-bar" style="width: 90%"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between mb-2">
                                <span class="text-gray-700">Vue.js</span>
                                <span class="text-gray-600">85%</span>
                            </div>
                            <div class="bg-gray-200 rounded-full h-2">
                                <div class="skill-bar" style="width: 85%"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between mb-2">
                                <span class="text-gray-700">CSS/Sass/Tailwind</span>
                                <span class="text-gray-600">92%</span>
                            </div>
                            <div class="bg-gray-200 rounded-full h-2">
                                <div class="skill-bar" style="width: 92%"></div>
                            </div>
                        </div>
                    </div>
                </div>
                
                <!-- Backend Skills -->
                <div class="bg-gray-50 rounded-lg p-8 card-hover">
                    <div class="text-center mb-6">
                        <i class="fas fa-server text-purple-600 text-4xl mb-4"></i>
                        <h3 class="text-xl font-semibold text-gray-800">Backend Development</h3>
                    </div>
                    <div class="space-y-4">
                        <div>
                            <div class="flex justify-between mb-2">
                                <span class="text-gray-700">Node.js</span>
                                <span class="text-gray-600">88%</span>
                            </div>
                            <div class="bg-gray-200 rounded-full h-2">
                                <div class="skill-bar" style="width: 88%"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between mb-2">
                                <span class="text-gray-700">Python/Django</span>
                                <span class="text-gray-600">82%</span>
                            </div>
                            <div class="bg-gray-200 rounded-full h-2">
                                <div class="skill-bar" style="width: 82%"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between mb-2">
                                <span class="text-gray-700">MongoDB/PostgreSQL</span>
                                <span class="text-gray-600">85%</span>
                            </div>
                            <div class="bg-gray-200 rounded-full h-2">
                                <div class="skill-bar" style="width: 85%"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between mb-2">
                                <span class="text-gray-700">REST APIs/GraphQL</span>
                                <span class="text-gray-600">90%</span>
                            </div>
                            <div class="bg-gray-200 rounded-full h-2">
                                <div class="skill-bar" style="width: 90%"></div>
                            </div>
                        </div>
                    </div>
                </div>
                
                <!-- Tools & Others -->
                <div class="bg-gray-50 rounded-lg p-8 card-hover">
                    <div class="text-center mb-6">
                        <i class="fas fa-tools text-purple-600 text-4xl mb-4"></i>
                        <h3 class="text-xl font-semibold text-gray-800">Tools & Others</h3>
                    </div>
                    <div class="space-y-4">
                        <div>
                            <div class="flex justify-between mb-2">
                                <span class="text-gray-700">Git/GitHub</span>
                                <span class="text-gray-600">95%</span>
                            </div>
                            <div class="bg-gray-200 rounded-full h-2">
                                <div class="skill-bar" style="width: 95%"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between mb-2">
                                <span class="text-gray-700">Docker/AWS</span>
                                <span class="text-gray-600">78%</span>
                            </div>
                            <div class="bg-gray-200 rounded-full h-2">
                                <div class="skill-bar" style="width: 78%"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between mb-2">
                                <span class="text-gray-700">Webpack/Vite</span>
                                <span class="text-gray-600">80%</span>
                            </div>
                            <div class="bg-gray-200 rounded-full h-2">
                                <div class="skill-bar" style="width: 80%"></div>
                            </div>
                        </div>
                        <div>
                            <div class="flex justify-between mb-2">
                                <span class="text-gray-700">Testing (Jest/Cypress)</span>
                                <span class="text-gray-600">75%</span>
                            </div>
                            <div class="bg-gray-200 rounded-full h-2">
                                <div class="skill-bar" style="width: 75%"></div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Projects Section -->
    <section id="projects" class="py-20 bg-gray-50">
        <div class="container mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="text-4xl font-bold text-gray-800 mb-4">Featured Projects</h2>
                <div class="w-24 h-1 bg-gradient-to-r from-purple-500 to-blue-500 mx-auto"></div>
                <p class="text-gray-600 mt-4 max-w-2xl mx-auto">Here are some of my recent projects that showcase my skills and experience</p>
            </div>
            
            <div class="grid md:grid-cols-3 gap-8">
                <!-- Project 1 -->
                <div class="bg-white rounded-lg shadow-lg overflow-hidden card-hover">
                    <div class="project-image">
                        <i class="fas fa-shopping-cart"></i>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-semibold text-gray-800 mb-3">E-Commerce Platform</h3>
                        <p class="text-gray-600 mb-4">A full-stack e-commerce solution built with React, Node.js, and MongoDB. Features include user authentication, payment integration, and admin dashboard.</p>
                        <div class="flex flex-wrap gap-2 mb-4">
                            <span class="px-3 py-1 bg-blue-100 text-blue-800 rounded-full text-sm">React</span>
                            <span class="px-3 py-1 bg-green-100 text-green-800 rounded-full text-sm">Node.js</span>
                            <span class="px-3 py-1 bg-yellow-100 text-yellow-800 rounded-full text-sm">MongoDB</span>
                        </div>
                        <div class="flex space-x-4">
                            <a href="#" class="text-purple-600 hover:text-purple-800 font-medium">
                                <i class="fas fa-external-link-alt mr-1"></i>Live Demo
                            </a>
                            <a href="#" class="text-gray-600 hover:text-gray-800 font-medium">
                                <i class="fab fa-github mr-1"></i>GitHub
                            </a>
                        </div>
                    </div>
                </div>
                
                <!-- Project 2 -->
                <div class="bg-white rounded-lg shadow-lg overflow-hidden card-hover">
                    <div class="project-image">
                        <i class="fas fa-tasks"></i>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-semibold text-gray-800 mb-3">Task Management App</h3>
                        <p class="text-gray-600 mb-4">A collaborative task management application with real-time updates, built using Vue.js and Firebase. Includes team collaboration features and progress tracking.</p>
                        <div class="flex flex-wrap gap-2 mb-4">
                            <span class="px-3 py-1 bg-green-100 text-green-800 rounded-full text-sm">Vue.js</span>
                            <span class="px-3 py-1 bg-orange-100 text-orange-800 rounded-full text-sm">Firebase</span>
                            <span class="px-3 py-1 bg-purple-100 text-purple-800 rounded-full text-sm">Vuetify</span>
                        </div>
                        <div class="flex space-x-4">
                            <a href="#" class="text-purple-600 hover:text-purple-800 font-medium">
                                <i class="fas fa-external-link-alt mr-1"></i>Live Demo
                            </a>
                            <a href="#" class="text-gray-600 hover:text-gray-800 font-medium">
                                <i class="fab fa-github mr-1"></i>GitHub
                            </a>
                        </div>
                    </div>
                </div>
                
                <!-- Project 3 -->
                <div class="bg-white rounded-lg shadow-lg overflow-hidden card-hover">
                    <div class="project-image">
                        <i class="fas fa-chart-line"></i>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-semibold text-gray-800 mb-3">Analytics Dashboard</h3>
                        <p class="text-gray-600 mb-4">A comprehensive analytics dashboard for tracking business metrics, built with React and D3.js. Features interactive charts, data visualization, and export capabilities.</p>
                        <div class="flex flex-wrap gap-2 mb-4">
                            <span class="px-3 py-1 bg-blue-100 text-blue-800 rounded-full text-sm">React</span>
                            <span class="px-3 py-1 bg-red-100 text-red-800 rounded-full text-sm">D3.js</span>
                            <span class="px-3 py-1 bg-gray-100 text-gray-800 rounded-full text-sm">Express</span>
                        </div>
                        <div class="flex space-x-4">
                            <a href="#" class="text-purple-600 hover:text-purple-800 font-medium">
                                <i class="fas fa-external-link-alt mr-1"></i>Live Demo
                            </a>
                            <a href="#" class="text-gray-600 hover:text-gray-800 font-medium">
                                <i class="fab fa-github mr-1"></i>GitHub
                            </a>
                        </div>
                    </div>
                </div>
                
                <!-- Project 4 -->
                <div class="bg-white rounded-lg shadow-lg overflow-hidden card-hover">
                    <div class="project-image">
                        <i class="fas fa-mobile-alt"></i>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-semibold text-gray-800 mb-3">Weather App PWA</h3>
                        <p class="text-gray-600 mb-4">A Progressive Web App for weather forecasting with offline capabilities, push notifications, and geolocation features. Built with vanilla JavaScript and modern PWA standards.</p>
                        <div class="flex flex-wrap gap-2 mb-4">
                            <span class="px-3 py-1 bg-yellow-100 text-yellow-800 rounded-full text-sm">JavaScript</span>
                            <span class="px-3 py-1 bg-blue-100 text-blue-800 rounded-full text-sm">PWA</span>
                            <span class="px-3 py-1 bg-green-100 text-green-800 rounded-full text-sm">Service Workers</span>
                        </div>
                        <div class="flex space-x-4">
                            <a href="#" class="text-purple-600 hover:text-purple-800 font-medium">
                                <i class="fas fa-external-link-alt mr-1"></i>Live Demo
                            </a>
                            <a href="#" class="text-gray-600 hover:text-gray-800 font-medium">
                                <i class="fab fa-github mr-1"></i>GitHub
                            </a>
                        </div>
                    </div>
                </div>
                
                <!-- Project 5 -->
                <div class="bg-white rounded-lg shadow-lg overflow-hidden card-hover">
                    <div class="project-image">
                        <i class="fas fa-blog"></i>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-semibold text-gray-800 mb-3">Personal Blog CMS</h3>
                        <p class="text-gray-600 mb-4">A custom content management system for blogs with markdown support, SEO optimization, and comment system. Built with Next.js and deployed on Vercel.</p>
                        <div class="flex flex-wrap gap-2 mb-4">
                            <span class="px-3 py-1 bg-black text-white rounded-full text-sm">Next.js</span>
                            <span class="px-3 py-1 bg-blue-100 text-blue-800 rounded-full text-sm">Markdown</span>
                            <span class="px-3 py-1 bg-green-100 text-green-800 rounded-full text-sm">Vercel</span>
                        </div>
                        <div class="flex space-x-4">
                            <a href="#" class="text-purple-600 hover:text-purple-800 font-medium">
                                <i class="fas fa-external-link-alt mr-1"></i>Live Demo
                            </a>
                            <a href="#" class="text-gray-600 hover:text-gray-800 font-medium">
                                <i class="fab fa-github mr-1"></i>GitHub
                            </a>
                        </div>
                    </div>
                </div>
                
                <!-- Project 6 -->
                <div class="bg-white rounded-lg shadow-lg overflow-hidden card-hover">
                    <div class="project-image">
                        <i class="fas fa-gamepad"></i>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-semibold text-gray-800 mb-3">Online Gaming Platform</h3>
                        <p class="text-gray-600 mb-4">A multiplayer gaming platform with real-time gameplay, user profiles, and leaderboards. Features WebSocket connections and responsive design for all devices.</p>
                        <div class="flex flex-wrap gap-2 mb-4">
                            <span class="px-3 py-1 bg-red-100 text-red-800 rounded-full text-sm">Socket.io</span>
                            <span class="px-3 py-1 bg-blue-100 text-blue-800 rounded-full text-sm">React</span>
                            <span class="px-3 py-1 bg-green-100 text-green-800 rounded-full text-sm">Node.js</span>
                        </div>
                        <div class="flex space-x-4">
                            <a href="#" class="text-purple-600 hover:text-purple-800 font-medium">
                                <i class="fas fa-external-link-alt mr-1"></i>Live Demo
                            </a>
                            <a href="#" class="text-gray-600 hover:text-gray-800 font-medium">
                                <i class="fab fa-github mr-1"></i>GitHub
                            </a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-20 bg-white">
        <div class="container mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="text-4xl font-bold text-gray-800 mb-4">Get In Touch</h2>
                <div class="w-24 h-1 bg-gradient-to-r from-purple-500 to-blue-500 mx-auto"></div>
                <p class="text-gray-600 mt-4 max-w-2xl mx-auto">I'm always open to discussing new opportunities, interesting projects, or just having a chat about technology</p>
            </div>
            
            <div class="grid md:grid-cols-2 gap-12 max-w-4xl mx-auto">
                <div class="space-y-8">
                    <div class="flex items-center space-x-4">
                        <div class="bg-purple-100 p-3 rounded-full">
                            <i class="fas fa-envelope text-purple-600 text-xl"></i>
                        </div>
                        <div>
                            <h4 class="font-semibold text-gray-800">Email</h4>
                            <p class="text-gray-600">alex.johnson@email.com</p>
                        </div>
                    </div>
                    
                    <div class="flex items-center space-x-4">
                        <div class="bg-purple-100 p-3 rounded-full">
                            <i class="fas fa-phone text-purple-600 text-xl"></i>
                        </div>
                        <div>
                            <h4 class="font-semibold text-gray-800">Phone</h4>
                            <p class="text-gray-600">+1 (555) 123-4567</p>
                        </div>
                    </div>
                    
                    <div class="flex items-center space-x-4">
                        <div class="bg-purple-100 p-3 rounded-full">
                            <i class="fas fa-map-marker-alt text-purple-600 text-xl"></i>
                        </div>
                        <div>
                            <h4 class="font-semibold text-gray-800">Location</h4>
                            <p class="text-gray-600">San Francisco, CA</p>
                        </div>
                    </div>
                    
                    <div class="pt-8">
                        <h4 class="font-semibold text-gray-800 mb-4">Connect With Me</h4>
                        <div class="flex space-x-4">
                            <a href="#" class="bg-gray-100 hover:bg-purple-100 p-3 rounded-full transition">
                                <i class="fab fa-linkedin text-xl text-gray-600 hover:text-purple-600"></i>
                            </a>
                            <a href="#" class="bg-gray-100 hover:bg-purple-100 p-3 rounded-full transition">
                                <i class="fab fa-github text-xl text-gray-600 hover:text-purple-600"></i>
                            </a>
                            <a href="#" class="bg-gray-100 hover:bg-purple-100 p-3 rounded-full transition">
                                <i class="fab fa-twitter text-xl text-gray-600 hover:text-purple-600"></i>
                            </a>
                            <a href="#" class="bg-gray-100 hover:bg-purple-100 p-3 rounded-full transition">
                                <i class="fab fa-dribbble text-xl text-gray-600 hover:text-purple-600"></i>
                            </a>
                        </div>
                    </div>
                </div>
                
                <div class="bg-gray-50 rounded-lg p-8">
                    <form class="space-y-6">
                        <div>
                            <label class="block text-gray-700 font-medium mb-2">Name</label>
                            <input type="text" class="w-full px-4 py-3 rounded-lg border border-gray-300 focus:border-purple-500 focus:outline-none transition">
                        </div>
                        <div>
                            <label class="block text-gray-700 font-medium mb-2">Email</label>
                            <input type="email" class="w-full px-4 py-3 rounded-lg border border-gray-300 focus:border-purple-500 focus:outline-none transition">
                        </div>
                        <div>
                            <label class="block text-gray-700 font-medium mb-2">Subject</label>
                            <input type="text" class="w-full px-4 py-3 rounded-lg border border-gray-300 focus:border-purple-500 focus:outline-none transition">
                        </div>
                        <div>
                            <label class="block text-gray-700 font-medium mb-2">Message</label>
                            <textarea rows="5" class="w-full px-4 py-3 rounded-lg border border-gray-300 focus:border-purple-500 focus:outline-none transition resize-none"></textarea>
                        </div>
                        <button type="submit" class="w-full bg-purple-600 text-white py-3 rounded-lg font-semibold hover:bg-purple-700 transition">
                            Send Message
                        </button>
                    </form>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="gradient-bg text-white py-8">
        <div class="container mx-auto px-6">
            <div class="flex flex-col md:flex-row justify-between items-center">
                <div class="mb-4 md:mb-0">
                    <p>&copy; 2024 Alex Johnson. All rights reserved.</p>
                </div>
                <div class="flex space-x-6">
                    <a href="#home" class="hover:text-purple-200 transition">Home</a>
                    <a href="#about" class="hover:text-purple-200 transition">About</a>
                    <a href="#skills" class="hover:text-purple-200 transition">Skills</a>
                    <a href="#projects" class="hover:text-purple-200 transition">Projects</a>
                    <a href="#contact" class="hover:text-purple-200 transition">Contact</a>
                </div>
            </div>
        </div>
    </footer>

    <script>
        // Smooth scrolling for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                }
            });
        });

        // Animate skill bars when they come into view
        const observerOptions = {
            threshold: 0.7
        };

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    const skillBars = entry.target.querySelectorAll('.skill-bar');
                    skillBars.forEach((bar, index) => {
                        setTimeout(() => {
                            bar.style.width = bar.style.width;
                        }, index * 200);
                    });
                }
            });
        }, observerOptions);

        document.querySelectorAll('#skills .card-hover').forEach(card => {
            observer.observe(card);
        });

        // Add active nav state
        window.addEventListener('scroll', () => {
            const sections = document.querySelectorAll('section[id]');
            const scrollPos = window.scrollY + 100;

            sections.forEach(section => {
                const top = section.offsetTop;
                const bottom = top + section.offsetHeight;
                const id = section.getAttribute('id');
                
                if (scrollPos >= top && scrollPos < bottom) {
                    document.querySelector(`nav a[href="#${id}"]`)?.classList.add('text-purple-600');
                } else {
                    document.querySelector(`nav a[href="#${id}"]`)?.classList.remove('text-purple-600');
                }
            });
        });

        // Form submission
        document.querySelector('form').addEventListener('submit', function(e) {
            e.preventDefault();
            alert('Thank you for your message! I\'ll get back to you soon.');
            this.reset();
        });
    </script>
</body>
</html>
