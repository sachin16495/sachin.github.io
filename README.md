<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sachin Pandey | Data Scientist Portfolio</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary: #2c3e50;
            --secondary: #3498db;
            --accent: #e74c3c;
            --light: #ecf0f1;
            --dark: #2c3e50;
            --success: #2ecc71;
            --text: #333;
            --card-bg: #fff;
            --card-shadow: 0 4px 8px rgba(0,0,0,0.1);
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: #f5f7fa;
            color: var(--text);
            line-height: 1.6;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        header {
            background: linear-gradient(135deg, var(--primary) 0%, var(--secondary) 100%);
            color: white;
            padding: 40px 0;
            text-align: center;
            position: relative;
            overflow: hidden;
        }

        .header-content {
            position: relative;
            z-index: 1;
        }

        .profile-img {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            border: 4px solid white;
            margin: 0 auto 20px;
            background-color: #ccc;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 60px;
            color: white;
        }

        h1 {
            font-size: 2.5rem;
            margin-bottom: 10px;
        }

        .tagline {
            font-size: 1.2rem;
            font-weight: 300;
            margin-bottom: 20px;
        }

        .contact-info {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 20px;
            margin-top: 20px;
        }

        .contact-item {
            display: flex;
            align-items: center;
            gap: 8px;
        }

        .section {
            padding: 60px 0;
        }

        .section-title {
            text-align: center;
            margin-bottom: 40px;
            color: var(--primary);
            position: relative;
        }

        .section-title:after {
            content: '';
            display: block;
            width: 60px;
            height: 4px;
            background: var(--secondary);
            margin: 10px auto;
        }

        .card {
            background: var(--card-bg);
            border-radius: 10px;
            box-shadow: var(--card-shadow);
            padding: 25px;
            margin-bottom: 25px;
            transition: transform 0.3s ease;
        }

        .card:hover {
            transform: translateY(-5px);
        }

        .card-title {
            color: var(--secondary);
            margin-bottom: 15px;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .timeline {
            position: relative;
            padding-left: 30px;
        }

        .timeline:before {
            content: '';
            position: absolute;
            left: 0;
            top: 0;
            height: 100%;
            width: 4px;
            background: var(--secondary);
        }

        .timeline-item {
            position: relative;
            margin-bottom: 30px;
        }

        .timeline-item:last-child {
            margin-bottom: 0;
        }

        .timeline-item:before {
            content: '';
            position: absolute;
            left: -38px;
            top: 5px;
            width: 20px;
            height: 20px;
            border-radius: 50%;
            background: var(--secondary);
            border: 4px solid var(--light);
        }

        .timeline-date {
            font-weight: 600;
            color: var(--secondary);
            margin-bottom: 5px;
        }

        .skills-container {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 20px;
        }

        .skill-category {
            margin-bottom: 20px;
        }

        .skill-list {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
        }

        .skill-tag {
            background: var(--light);
            padding: 8px 15px;
            border-radius: 20px;
            font-size: 0.9rem;
            display: inline-block;
            margin-bottom: 8px;
            transition: all 0.3s ease;
        }

        .skill-tag:hover {
            background: var(--secondary);
            color: white;
            cursor: default;
        }

        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 25px;
        }

        .project-card {
            height: 100%;
            display: flex;
            flex-direction: column;
        }

        .project-title {
            color: var(--primary);
            margin-bottom: 10px;
        }

        .project-tech {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
            margin: 10px 0;
        }

        .tech-tag {
            background: var(--light);
            padding: 5px 10px;
            border-radius: 15px;
            font-size: 0.8rem;
        }

        .achievements-list {
            list-style-type: none;
        }

        .achievements-list li {
            margin-bottom: 15px;
            padding-left: 30px;
            position: relative;
        }

        .achievements-list li:before {
            content: '★';
            position: absolute;
            left: 0;
            color: var(--accent);
        }

        footer {
            background: var(--dark);
            color: white;
            text-align: center;
            padding: 30px 0;
        }

        .social-links {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin: 20px 0;
        }

        .social-links a {
            color: white;
            font-size: 1.5rem;
            transition: color 0.3s ease;
        }

        .social-links a:hover {
            color: var(--secondary);
        }

        @media (max-width: 768px) {
            .skills-container {
                grid-template-columns: 1fr;
            }
            
            .projects-grid {
                grid-template-columns: 1fr;
            }
            
            .contact-info {
                flex-direction: column;
                align-items: center;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <div class="header-content">
                <div class="profile-img">
                    <i class="fas fa-user"></i>
                </div>
                <h1>Sachin Pandey</h1>
                <p class="tagline">Data Scientist & AI Specialist | LLM Expert | 7+ Years Experience</p>
                <div class="contact-info">
                    <div class="contact-item">
                        <i class="fas fa-phone"></i>
                        <span>+91 9140067500</span>
                    </div>
                    <div class="contact-item">
                        <i class="fas fa-envelope"></i>
                        <span>spsachin.official@gmail.com</span>
                    </div>
                    <div class="contact-item">
                        <i class="fas fa-map-marker-alt"></i>
                        <span>Bengaluru, Karnataka, India</span>
                    </div>
                </div>
            </div>
        </div>
    </header>

    <section class="section" id="intro">
        <div class="container">
            <h2 class="section-title">Introduction</h2>
            <div class="card">
                <p>AI professional with 7+ years as a Data Scientist, including 3 years in LLM, LLM evaluation and responsible AI. Expertise in designing evaluation strategies, metrics, OKRs, and automated pipelines to optimize performance, cost, and user experience. Proven skills in program management, stakeholder engagement, and LLM research.</p>
                <p>Delivered and deployed 2 agentic models, 5 RAG-based LLMs, 5 fine-tuned LLMs, and 8 ML/DL models; holder of a patent in LLM innovation.</p>
            </div>
        </div>
    </section>

    <section class="section" id="experience">
        <div class="container">
            <h2 class="section-title">Work Experience</h2>
            <div class="timeline">
                <div class="timeline-item">
                    <div class="card">
                        <div class="timeline-date">2024 - Present</div>
                        <h3 class="card-title"><i class="fas fa-briefcase"></i> Manager Data Scientist [Gen AI Engineer] - Concentrix</h3>
                        <ul>
                            <li>Generate strategic documentation generator using RAG by processing meeting notes and OONG call data through an LLM model</li>
                            <li>Developed custom content generation Agent using Langgraph</li>
                            <li>Develop a social listening agent using Langgraph for Linkedin Marketing solution</li>
                            <li>Fine-tuned a Llama model and implemented RAG to develop a Q&A system for tender documents</li>
                            <li>Designed and implemented a Multi-Hop RAG system for legal contracts</li>
                            <li>Developed an end-to-end AIOps solution using a streaming architecture</li>
                        </ul>
                    </div>
                </div>
                <div class="timeline-item">
                    <div class="card">
                        <div class="timeline-date">2021 - 2024</div>
                        <h3 class="card-title"><i class="fas fa-briefcase"></i> Data Scientist - II - Concentrix</h3>
                        <ul>
                            <li>Fine-tuning Mistral 78 Base Model with CLOFA on transaction data</li>
                            <li>Filed a patent for Transaction classification model using LLM</li>
                            <li>Use Mistral Instruct to extract the entity with RAG</li>
                            <li>Automated the labeling process using GPT model and Langchain</li>
                            <li>Solved Financial Institute Transaction categorization problem using BERT Model</li>
                        </ul>
                    </div>
                </div>
                <div class="timeline-item">
                    <div class="card">
                        <div class="timeline-date">2020 - 2021</div>
                        <h3 class="card-title"><i class="fas fa-briefcase"></i> Data Scientist - Arya</h3>
                        <ul>
                            <li>Automated the insurance underwriting process using deep learning</li>
                            <li>Build an Early/fraud claims during underwriting</li>
                            <li>Build an ICD Classifier model using BERT and elasticsearch</li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section class="section" id="skills">
        <div class="container">
            <h2 class="section-title">Skills & Expertise</h2>
            <div class="skills-container">
                <div class="card">
                    <h3 class="card-title"><i class="fas fa-code"></i> Programming</h3>
                    <div class="skill-list">
                        <span class="skill-tag">Python</span>
                        <span class="skill-tag">SQL</span>
                        <span class="skill-tag">TensorFlow</span>
                    </div>
                </div>
                <div class="card">
                    <h3 class="card-title"><i class="fas fa-brain"></i> AI/ML Technologies</h3>
                    <div class="skill-list">
                        <span class="skill-tag">Machine Learning</span>
                        <span class="skill-tag">Deep Learning</span>
                        <span class="skill-tag">Natural Language Processing</span>
                        <span class="skill-tag">LLM</span>
                        <span class="skill-tag">Generative AI</span>
                        <span class="skill-tag">Agentic AI</span>
                        <span class="skill-tag">RAG</span>
                    </div>
                </div>
                <div class="card">
                    <h3 class="card-title"><i class="fas fa-tools"></i> Tools & Platforms</h3>
                    <div class="skill-list">
                        <span class="skill-tag">Docker</span>
                        <span class="skill-tag">Kubernetes</span>
                        <span class="skill-tag">HDFS</span>
                        <span class="skill-tag">Langchain</span>
                        <span class="skill-tag">Langgraph</span>
                        <span class="skill-tag">CI/CD Pipeline</span>
                    </div>
                </div>
                <div class="card">
                    <h3 class="card-title"><i class="fas fa-eye"></i> Domains</h3>
                    <div class="skill-list">
                        <span class="skill-tag">Computer Vision</span>
                        <span class="skill-tag">Responsible AI</span>
                        <span class="skill-tag">AIOps</span>
                        <span class="skill-tag">Financial Systems</span>
                        <span class="skill-tag">Insurance</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section class="section" id="achievements">
        <div class="container">
            <h2 class="section-title">Achievements</h2>
            <div class="card">
                <ul class="achievements-list">
                    <li>Holder of a patent in LLM innovation for transaction classification</li>
                    <li>Delivered and deployed 2 agentic models in production environments</li>
                    <li>Developed and implemented 5 RAG-based LLM systems</li>
                    <li>Fine-tuned and deployed 5 LLM models for specific business use cases</li>
                    <li>Built and deployed 8 ML/DL models solving real-world business problems</li>
                    <li>Successfully automated insurance underwriting process with high precision metrics</li>
                </ul>
            </div>
        </div>
    </section>

    <section class="section" id="projects">
        <div class="container">
            <h2 class="section-title">Projects</h2>
            <div class="projects-grid">
                <div class="card project-card">
                    <h3 class="project-title">Strategic Documentation Generator</h3>
                    <p>RAG-based system processing meeting notes and call data through LLM</p>
                    <div class="project-tech">
                        <span class="tech-tag">Gen AI</span>
                        <span class="tech-tag">RAG</span>
                        <span class="tech-tag">Langchain</span>
                    </div>
                </div>
                <div class="card project-card">
                    <h3 class="project-title">Content Generation Agent</h3>
                    <p>Custom agent using Langgraph leveraging audience insights</p>
                    <div class="project-tech">
                        <span class="tech-tag">Agentic AI</span>
                        <span class="tech-tag">Langgraph</span>
                    </div>
                </div>
                <div class="card project-card">
                    <h3 class="project-title">Social Listening Agent</h3>
                    <p>LinkedIn Marketing solution for topic detection and sentiment extraction</p>
                    <div class="project-tech">
                        <span class="tech-tag">Agentic AI</span>
                        <span class="tech-tag">Gen AI</span>
                        <span class="tech-tag">Function Calling</span>
                    </div>
                </div>
                <div class="card project-card">
                    <h3 class="project-title">Tender Document Q&A System</h3>
                    <p>Fine-tuned Llama model with RAG for tender documents</p>
                    <div class="project-tech">
                        <span class="tech-tag">VLIM</span>
                        <span class="tech-tag">CLOFA</span>
                        <span class="tech-tag">Llama</span>
                    </div>
                </div>
                <div class="card project-card">
                    <h3 class="project-title">Multi-Hop RAG System</h3>
                    <p>Structured representations of legal contracts with DataFrame agent</p>
                    <div class="project-tech">
                        <span class="tech-tag">RAG</span>
                        <span class="tech-tag">Chunking</span>
                        <span class="tech-tag">OpenAI</span>
                    </div>
                </div>
                <div class="card project-card">
                    <h3 class="project-title">AIOps Solution</h3>
                    <p>Streaming architecture for real-time log processing and anomaly detection</p>
                    <div class="project-tech">
                        <span class="tech-tag">Kafka</span>
                        <span class="tech-tag">Fast API</span>
                        <span class="tech-tag">Docker</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <footer>
        <div class="container">
            <h3>Connect with Me</h3>
            <div class="social-links">
                <a href="https://github.com/sachin16495" target="_blank"><i class="fab fa-github"></i></a>
                <a href="mailto:spsachin.official@gmail.com"><i class="fas fa-envelope"></i></a>
                <a href="#"><i class="fab fa-linkedin"></i></a>
                <a href="#"><i class="fab fa-twitter"></i></a>
            </div>
            <p>© 2023 Sachin Pandey. All rights reserved.</p>
        </div>
    </footer>

    <script>
        // Simple animation for elements when they come into view
        document.addEventListener('DOMContentLoaded', function() {
            const cards = document.querySelectorAll('.card');
            
            const observer = new IntersectionObserver((entries) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.style.opacity = 1;
                        entry.target.style.transform = 'translateY(0)';
                    }
                });
            }, { threshold: 0.1 });
            
            cards.forEach(card => {
                card.style.opacity = 0;
                card.style.transform = 'translateY(20px)';
                card.style.transition = 'opacity 0.5s ease, transform 0.5s ease';
                observer.observe(card);
            });
        });
    </script>
</body>
</html>
