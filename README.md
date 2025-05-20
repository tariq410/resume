# resume
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Create professional, downloadable resumes for free. Our resume builder helps you craft the perfect CV with dynamic templates and easy customization.">
    <meta name="keywords" content="resume builder, CV creator, professional resume, job application, resume template">
    <meta name="author" content="Resume Creator Pro">
    <meta property="og:title" content="Free Online Resume Builder | Professional CV Creator">
    <meta property="og:description" content="Create and download professional resumes in minutes with our free resume builder.">
    <meta property="og:type" content="website">
    <meta property="og:url" content="https://www.yourresumebuilder.com">
    <meta name="robots" content="index, follow">
    <link rel="canonical" href="https://www.yourresumebuilder.com">
    <title>Free Online Resume Builder | Create & Download Professional CV</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;500;700&family=Poppins:wght@400;600;700&display=swap" rel="stylesheet">
    <script src="https://cdnjs.cloudflare.com/ajax/libs/html2pdf.js/0.10.1/html2pdf.bundle.min.js" integrity="sha512-GsLlZN/3F2ErC5ifS5QtgpiJtWd43JWSuIgh7mbzZ8zBps+dvLusV+eNQATqgA/HdeKFVgA5v3S/cIrLF7QnIg==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
    <style>
        :root {
            --primary-color: #3498db;
            --secondary-color: #2980b9;
            --accent-color: #e74c3c;
            --light-color: #ecf0f1;
            --dark-color: #2c3e50;
            --text-color: #333;
            --text-light: #7f8c8d;
            --shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            --transition: all 0.3s ease;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Roboto', sans-serif;
            line-height: 1.6;
            color: var(--text-color);
            background-color: #f5f7fa;
            overflow-x: hidden;
        }

        header {
            background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
            color: white;
            padding: 1.5rem 0;
            box-shadow: var(--shadow);
            position: relative;
            z-index: 100;
        }

        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 15px;
        }

        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-family: 'Poppins', sans-serif;
            font-weight: 700;
            font-size: 1.8rem;
            display: flex;
            align-items: center;
        }

        .logo i {
            margin-right: 10px;
            font-size: 2rem;
        }

        nav ul {
            display: flex;
            list-style: none;
        }

        nav ul li {
            margin-left: 1.5rem;
        }

        nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: 500;
            transition: var(--transition);
            padding: 0.5rem 0;
            position: relative;
        }

        nav ul li a:hover {
            opacity: 0.9;
        }

        nav ul li a::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 0;
            height: 2px;
            background-color: white;
            transition: var(--transition);
        }

        nav ul li a:hover::after {
            width: 100%;
        }

        .mobile-menu-btn {
            display: none;
            background: none;
            border: none;
            color: white;
            font-size: 1.5rem;
            cursor: pointer;
        }

        .hero {
            padding: 4rem 0;
            text-align: center;
            background-color: white;
        }

        .hero h1 {
            font-size: 2.5rem;
            margin-bottom: 1rem;
            color: var(--dark-color);
            font-family: 'Poppins', sans-serif;
        }

        .hero p {
            font-size: 1.1rem;
            color: var(--text-light);
            max-width: 700px;
            margin: 0 auto 2rem;
        }

        .cta-button {
            display: inline-block;
            background-color: var(--accent-color);
            color: white;
            padding: 0.8rem 2rem;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 500;
            transition: var(--transition);
            border: none;
            cursor: pointer;
            font-size: 1rem;
            box-shadow: var(--shadow);
        }

        .cta-button:hover {
            background-color: #c0392b;
            transform: translateY(-3px);
        }

        .main-content {
            display: flex;
            flex-wrap: wrap;
            gap: 2rem;
            padding: 2rem 0;
        }

        .form-section {
            flex: 1;
            min-width: 300px;
            background-color: white;
            border-radius: 8px;
            padding: 2rem;
            box-shadow: var(--shadow);
        }

        .preview-section {
            flex: 1;
            min-width: 300px;
            background-color: white;
            border-radius: 8px;
            padding: 2rem;
            box-shadow: var(--shadow);
            position: relative;
        }

        .section-title {
            font-family: 'Poppins', sans-serif;
            font-size: 1.5rem;
            margin-bottom: 1.5rem;
            color: var(--dark-color);
            position: relative;
            padding-bottom: 0.5rem;
        }

        .section-title::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 50px;
            height: 3px;
            background-color: var(--primary-color);
        }

        .form-group {
            margin-bottom: 1.5rem;
        }

        label {
            display: block;
            margin-bottom: 0.5rem;
            font-weight: 500;
        }

        input, textarea, select {
            width: 100%;
            padding: 0.8rem;
            border: 1px solid #ddd;
            border-radius: 4px;
            font-family: inherit;
            font-size: 1rem;
            transition: var(--transition);
        }

        input:focus, textarea:focus, select:focus {
            outline: none;
            border-color: var(--primary-color);
            box-shadow: 0 0 0 2px rgba(52, 152, 219, 0.2);
        }

        textarea {
            min-height: 100px;
            resize: vertical;
        }

        .form-row {
            display: flex;
            gap: 1rem;
        }

        .form-row .form-group {
            flex: 1;
        }

        .add-btn, .remove-btn {
            background-color: var(--light-color);
            color: var(--text-color);
            border: none;
            padding: 0.5rem 1rem;
            border-radius: 4px;
            cursor: pointer;
            font-size: 0.9rem;
            transition: var(--transition);
            display: inline-flex;
            align-items: center;
            margin-top: 0.5rem;
        }

        .add-btn:hover, .remove-btn:hover {
            background-color: #ddd;
        }

        .add-btn i, .remove-btn i {
            margin-right: 5px;
        }

        .resume {
            font-family: 'Roboto', sans-serif;
            background-color: white;
            padding: 2rem;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            max-width: 800px;
            margin: 0 auto;
        }

        .resume-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 1.5rem;
            padding-bottom: 1rem;
            border-bottom: 2px solid var(--primary-color);
        }

        .resume-name {
            font-size: 2rem;
            font-weight: 700;
            color: var(--dark-color);
            margin-bottom: 0.5rem;
        }

        .resume-title {
            font-size: 1.2rem;
            color: var(--primary-color);
            font-weight: 500;
        }

        .resume-contact {
            text-align: right;
        }

        .resume-contact p {
            margin-bottom: 0.3rem;
            font-size: 0.9rem;
        }

        .resume-section {
            margin-bottom: 1.5rem;
        }

        .resume-section-title {
            font-size: 1.3rem;
            font-weight: 600;
            color: var(--dark-color);
            margin-bottom: 0.5rem;
            padding-bottom: 0.3rem;
            border-bottom: 1px solid #eee;
        }

        .resume-item {
            margin-bottom: 1rem;
        }

        .resume-item-header {
            display: flex;
            justify-content: space-between;
            margin-bottom: 0.3rem;
        }

        .resume-item-title {
            font-weight: 600;
            font-size: 1.1rem;
        }

        .resume-item-date {
            color: var(--text-light);
            font-size: 0.9rem;
        }

        .resume-item-subtitle {
            font-style: italic;
            color: var(--text-light);
            margin-bottom: 0.3rem;
            font-size: 0.9rem;
        }

        .resume-item-description {
            font-size: 0.95rem;
            line-height: 1.5;
        }

        .skills-list {
            display: flex;
            flex-wrap: wrap;
            gap: 0.5rem;
        }

        .skill-tag {
            background-color: var(--light-color);
            padding: 0.3rem 0.8rem;
            border-radius: 20px;
            font-size: 0.9rem;
        }

        .action-buttons {
            display: flex;
            justify-content: center;
            gap: 1rem;
            margin-top: 2rem;
        }

        .download-btn {
            background-color: var(--primary-color);
            color: white;
        }

        .download-btn:hover {
            background-color: var(--secondary-color);
        }

        .reset-btn {
            background-color: var(--light-color);
            color: var(--text-color);
        }

        .reset-btn:hover {
            background-color: #ddd;
        }

        .ad-container {
            background-color: #f9f9f9;
            border: 1px solid #eee;
            padding: 1rem;
            margin: 2rem 0;
            text-align: center;
            border-radius: 4px;
        }

        .ad-label {
            font-size: 0.8rem;
            color: var(--text-light);
            margin-bottom: 0.5rem;
            text-transform: uppercase;
        }

        .testimonials {
            padding: 3rem 0;
            background-color: var(--light-color);
        }

        .testimonials h2 {
            text-align: center;
            margin-bottom: 2rem;
            font-family: 'Poppins', sans-serif;
            color: var(--dark-color);
        }

        .testimonial-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }

        .testimonial-card {
            background-color: white;
            padding: 1.5rem;
            border-radius: 8px;
            box-shadow: var(--shadow);
        }

        .testimonial-text {
            font-style: italic;
            margin-bottom: 1rem;
            position: relative;
        }

        .testimonial-text::before {
            content: '"';
            font-size: 3rem;
            color: var(--primary-color);
            opacity: 0.2;
            position: absolute;
            top: -1rem;
            left: -1rem;
        }

        .testimonial-author {
            font-weight: 600;
            color: var(--primary-color);
        }

        .feedback-section {
            padding: 3rem 0;
            background-color: white;
        }

        .feedback-section h2 {
            text-align: center;
            margin-bottom: 2rem;
            font-family: 'Poppins', sans-serif;
            color: var(--dark-color);
        }

        .feedback-form {
            max-width: 600px;
            margin: 0 auto;
            background-color: var(--light-color);
            padding: 2rem;
            border-radius: 8px;
            box-shadow: var(--shadow);
        }

        .rating-container {
            display: flex;
            justify-content: center;
            margin-bottom: 1.5rem;
        }

        .rating-input {
            display: none;
        }

        .rating-label {
            font-size: 2rem;
            color: #ddd;
            cursor: pointer;
            transition: var(--transition);
            margin: 0 0.2rem;
        }

        .rating-input:checked ~ .rating-label,
        .rating-label:hover,
        .rating-label:hover ~ .rating-label {
            color: #f1c40f;
        }

        footer {
            background-color: var(--dark-color);
            color: white;
            padding: 2rem 0;
            text-align: center;
        }

        .footer-content {
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        .footer-links {
            display: flex;
            gap: 1.5rem;
            margin: 1.5rem 0;
        }

        .footer-links a {
            color: white;
            text-decoration: none;
            transition: var(--transition);
        }

        .footer-links a:hover {
            color: var(--primary-color);
        }

        .social-icons {
            display: flex;
            gap: 1rem;
            margin-bottom: 1.5rem;
        }

        .social-icon {
            width: 40px;
            height: 40px;
            border-radius: 50%;
            background-color: rgba(255, 255, 255, 0.1);
            display: flex;
            align-items: center;
            justify-content: center;
            transition: var(--transition);
        }

        .social-icon:hover {
            background-color: var(--primary-color);
            transform: translateY(-3px);
        }

        .copyright {
            font-size: 0.9rem;
            color: rgba(255, 255, 255, 0.7);
        }

        @media (max-width: 768px) {
            .header-content {
                flex-direction: column;
                text-align: center;
            }

            nav ul {
                margin-top: 1rem;
                flex-direction: column;
                align-items: center;
            }

            nav ul li {
                margin: 0.5rem 0;
            }

            .hero h1 {
                font-size: 2rem;
            }

            .form-row {
                flex-direction: column;
                gap: 0;
            }

            .resume-header {
                flex-direction: column;
                align-items: flex-start;
            }

            .resume-contact {
                text-align: left;
                margin-top: 1rem;
            }

            .action-buttons {
                flex-direction: column;
            }

            .cta-button {
                width: 100%;
                margin-bottom: 1rem;
            }
        }

        @media (max-width: 480px) {
            .mobile-menu-btn {
                display: block;
            }

            nav {
                display: none;
                width: 100%;
                margin-top: 1rem;
            }

            nav.active {
                display: block;
            }

            .hero {
                padding: 2rem 0;
            }

            .hero h1 {
                font-size: 1.8rem;
            }

            .main-content {
                flex-direction: column;
            }

            .form-section, .preview-section {
                width: 100%;
            }
        }

        /* Print styles */
        @media print {
            body * {
                visibility: hidden;
            }
            .resume, .resume * {
                visibility: visible;
            }
            .resume {
                position: absolute;
                left: 0;
                top: 0;
                width: 100%;
                box-shadow: none;
                padding: 0;
            }
            .no-print {
                display: none;
            }
        }
    </style>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
</head>
<body>
    <header>
        <div class="container">
            <div class="header-content">
                <div class="logo">
                    <i class="fas fa-file-alt"></i>
                    <span>ResumeCreator</span>
                </div>
                <button class="mobile-menu-btn" id="mobileMenuBtn">
                    <i class="fas fa-bars"></i>
                </button>
                <nav id="mainNav">
                    <ul>
                        <li><a href="#features">Features</a></li>
                        <li><a href="#templates">Templates</a></li>
                        <li><a href="#testimonials">Testimonials</a></li>
                        <li><a href="#feedback">Feedback</a></li>
                    </ul>
                </nav>
            </div>
        </div>
    </header>

    <section class="hero">
        <div class="container">
            <h1>Create Your Professional Resume in Minutes</h1>
            <p>Our free resume builder helps you craft the perfect resume that gets you noticed by employers. Simply fill in your details, customize the design, and download your resume.</p>
            <a href="#builder" class="cta-button">Start Building Now</a>
        </div>
    </section>

    <!-- Ad Space -->
    <div class="container">
        <div class="ad-container">
            <div class="ad-label">Advertisement</div>
            <!-- Google AdSense Ad Unit -->
            <script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-pub-XXXXXXXXXXXXXXXX"
                crossorigin="anonymous"></script>
            <!-- Resume Builder Top Banner -->
            <ins class="adsbygoogle"
                style="display:block"
                data-ad-client="ca-pub-XXXXXXXXXXXXXXXX"
                data-ad-slot="XXXXXXXXXX"
                data-ad-format="auto"
                data-full-width-responsive="true"></ins>
            <script>
                (adsbygoogle = window.adsbygoogle || []).push({});
            </script>
        </div>
    </div>

    <main class="main-content" id="builder">
        <section class="form-section">
            <h2 class="section-title">Your Information</h2>
            
            <div class="form-group">
                <label for="fullName">Full Name</label>
                <input type="text" id="fullName" placeholder="John Doe">
            </div>
            
            <div class="form-group">
                <label for="jobTitle">Professional Title</label>
                <input type="text" id="jobTitle" placeholder="e.g. Web Developer">
            </div>
            
            <div class="form-group">
                <label for="professionalSummary">Professional Summary</label>
                <textarea id="professionalSummary" placeholder="Briefly describe your professional background and skills"></textarea>
            </div>
            
            <h3 class="section-title">Contact Information</h3>
            
            <div class="form-row">
                <div class="form-group">
                    <label for="email">Email</label>
                    <input type="email" id="email" placeholder="your.email@example.com">
                </div>
                <div class="form-group">
                    <label for="phone">Phone</label>
                    <input type="tel" id="phone" placeholder="(123) 456-7890">
                </div>
            </div>
            
            <div class="form-row">
                <div class="form-group">
                    <label for="address">Address</label>
                    <input type="text" id="address" placeholder="123 Main St, City">
                </div>
                <div class="form-group">
                    <label for="linkedin">LinkedIn</label>
                    <input type="url" id="linkedin" placeholder="https://linkedin.com/in/yourprofile">
                </div>
            </div>
            
            <div class="form-group">
                <label for="portfolio">Portfolio/GitHub</label>
                <input type="url" id="portfolio" placeholder="https://yourportfolio.com">
            </div>
            
            <h3 class="section-title">Work Experience</h3>
            <div id="experienceFields">
                <div class="experience-entry">
                    <div class="form-row">
                        <div class="form-group">
                            <label for="jobTitle1">Job Title</label>
                            <input type="text" id="jobTitle1" placeholder="Senior Developer">
                        </div>
                        <div class="form-group">
                            <label for="company1">Company</label>
                            <input type="text" id="company1" placeholder="Tech Corp Inc.">
                        </div>
                    </div>
                    
                    <div class="form-row">
                        <div class="form-group">
                            <label for="startDate1">Start Date</label>
                            <input type="text" id="startDate1" placeholder="MM/YYYY">
                        </div>
                        <div class="form-group">
                            <label for="endDate1">End Date</label>
                            <input type="text" id="endDate1" placeholder="MM/YYYY or Present">
                        </div>
                    </div>
                    
                    <div class="form-group">
                        <label for="jobDescription1">Job Description</label>
                        <textarea id="jobDescription1" placeholder="Describe your responsibilities and achievements"></textarea>
                    </div>
                </div>
            </div>
            
            <button type="button" class="add-btn" id="addExperience">
                <i class="fas fa-plus"></i> Add Another Position
            </button>
            
            <h3 class="section-title">Education</h3>
            <div id="educationFields">
                <div class="education-entry">
                    <div class="form-row">
                        <div class="form-group">
                            <label for="degree1">Degree</label>
                            <input type="text" id="degree1" placeholder="Bachelor of Science">
                        </div>
                        <div class="form-group">
                            <label for="university1">Institution</label>
                            <input type="text" id="university1" placeholder="University Name">
                        </div>
                    </div>
                    
                    <div class="form-row">
                        <div class="form-group">
                            <label for="educationStartDate1">Start Date</label>
                            <input type="text" id="educationStartDate1" placeholder="MM/YYYY">
                        </div>
                        <div class="form-group">
                            <label for="educationEndDate1">End Date</label>
                            <input type="text" id="educationEndDate1" placeholder="MM/YYYY or Present">
                        </div>
                    </div>
                    
                    <div class="form-group">
                        <label for="educationDescription1">Description</label>
                        <textarea id="educationDescription1" placeholder="Notable achievements, honors, or relevant coursework"></textarea>
                    </div>
                </div>
            </div>
            
            <button type="button" class="add-btn" id="addEducation">
                <i class="fas fa-plus"></i> Add Another Education
            </button>
            
            <h3 class="section-title">Skills</h3>
            <div class="form-group">
                <label for="skills">List your skills (comma separated)</label>
                <textarea id="skills" placeholder="JavaScript, HTML, CSS, Project Management, etc."></textarea>
            </div>
            
            <h3 class="section-title">Certifications</h3>
            <div id="certificationFields">
                <div class="certification-entry">
                    <div class="form-row">
                        <div class="form-group">
                            <label for="certificationName1">Certification Name</label>
                            <input type="text" id="certificationName1" placeholder="Certified Web Developer">
                        </div>
                        <div class="form-group">
                            <label for="certificationOrg1">Issuing Organization</label>
                            <input type="text" id="certificationOrg1" placeholder="Web Development Institute">
                        </div>
                    </div>
                    
                    <div class="form-group">
                        <label for="certificationYear1">Year Obtained</label>
                        <input type="text" id="certificationYear1" placeholder="YYYY">
                    </div>
                </div>
            </div>
            
            <button type="button" class="add-btn" id="addCertification">
                <i class="fas fa-plus"></i> Add Another Certification
            </button>
            
            <h3 class="section-title">Projects</h3>
            <div id="projectFields">
                <div class="project-entry">
                    <div class="form-group">
                        <label for="projectName1">Project Name</label>
                        <input type="text" id="projectName1" placeholder="E-commerce Website">
                    </div>
                    
                    <div class="form-group">
                        <label for="projectDescription1">Project Description</label>
                        <textarea id="projectDescription1" placeholder="Describe the project, your role, and technologies used"></textarea>
                    </div>
                    
                    <div class="form-group">
                        <label for="projectLink1">Project Link (optional)</label>
                        <input type="url" id="projectLink1" placeholder="https://projectdemo.com">
                    </div>
                </div>
            </div>
            
            <button type="button" class="add-btn" id="addProject">
                <i class="fas fa-plus"></i> Add Another Project
            </button>
        </section>
        
        <section class="preview-section">
            <h2 class="section-title">Resume Preview</h2>
            
            <div class="resume" id="resumePreview">
                <div class="resume-header">
                    <div>
                        <h1 class="resume-name" id="previewName">Your Name</h1>
                        <p class="resume-title" id="previewTitle">Professional Title</p>
                    </div>
                    <div class="resume-contact">
                        <p id="previewEmail">email@example.com</p>
                        <p id="previewPhone">(123) 456-7890</p>
                        <p id="previewAddress">123 Main St, City, State</p>
                        <p id="previewLinkedIn">linkedin.com/in/yourprofile</p>
                        <p id="previewPortfolio">yourportfolio.com</p>
                    </div>
                </div>
                
                <div class="resume-section">
                    <h3 class="resume-section-title">Professional Summary</h3>
                    <p id="previewSummary">Experienced professional with a proven track record in the industry. Skilled in various technologies and methodologies with a strong ability to adapt and learn quickly.</p>
                </div>
                
                <div class="resume-section">
                    <h3 class="resume-section-title">Work Experience</h3>
                    <div class="resume-item" id="previewExperience1">
                        <div class="resume-item-header">
                            <span class="resume-item-title">Job Title</span>
                            <span class="resume-item-date">MM/YYYY - MM/YYYY</span>
                        </div>
                        <p class="resume-item-subtitle">Company Name</p>
                        <p class="resume-item-description">Job responsibilities and achievements.</p>
                    </div>
                    <!-- More experience entries will be added here dynamically -->
                </div>
                
                <div class="resume-section">
                    <h3 class="resume-section-title">Education</h3>
                    <div class="resume-item" id="previewEducation1">
                        <div class="resume-item-header">
                            <span class="resume-item-title">Degree</span>
                            <span class="resume-item-date">MM/YYYY - MM/YYYY</span>
                        </div>
                        <p class="resume-item-subtitle">Institution Name</p>
                        <p class="resume-item-description">Notable achievements or coursework.</p>
                    </div>
                    <!-- More education entries will be added here dynamically -->
                </div>
                
                <div class="resume-section">
                    <h3 class="resume-section-title">Skills</h3>
                    <div class="skills-list" id="previewSkills">
                        <span class="skill-tag">Skill 1</span>
                        <span class="skill-tag">Skill 2</span>
                        <span class="skill-tag">Skill 3</span>
                    </div>
                </div>
                
                <div class="resume-section">
                    <h3 class="resume-section-title">Certifications</h3>
                    <div class="resume-item" id="previewCertification1">
                        <div class="resume-item-header">
                            <span class="resume-item-title">Certification Name</span>
                            <span class="resume-item-date">YYYY</span>
                        </div>
                        <p class="resume-item-subtitle">Issuing Organization</p>
                    </div>
                    <!-- More certification entries will be added here dynamically -->
                </div>
                
                <div class="resume-section">
                    <h3 class="resume-section-title">Projects</h3>
                    <div class="resume-item" id="previewProject1">
                        <div class="resume-item-header">
                            <span class="resume-item-title">Project Name</span>
                        </div>
                        <p class="resume-item-description">Project description and technologies used.</p>
                        <p class="resume-item-description"><a href="#" target="_blank">Project Link</a></p>
                    </div>
                    <!-- More project entries will be added here dynamically -->
                </div>
            </div>
            
            <div class="action-buttons">
                <button class="cta-button download-btn" id="downloadBtn">
                    <i class="fas fa-download"></i> Download Resume
                </button>
                <button class="cta-button reset-btn" id="resetBtn">
                    <i class="fas fa-redo"></i> Reset Form
                </button>
            </div>
        </section>
    </main>

    <!-- Mid-Page Ad Space -->
    <div class="container">
        <div class="ad-container">
            <div class="ad-label">Advertisement</div>
            <!-- Google AdSense Ad Unit -->
            <script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-pub-XXXXXXXXXXXXXXXX"
                crossorigin="anonymous"></script>
            <!-- Resume Builder Mid-Page Rectangle -->
            <ins class="adsbygoogle"
                style="display:block"
                data-ad-client="ca-pub-XXXXXXXXXXXXXXXX"
                data-ad-slot="XXXXXXXXXX"
                data-ad-format="auto"
                data-full-width-responsive="true"></ins>
            <script>
                (adsbygoogle = window.adsbygoogle || []).push({});
            </script>
        </div>
    </div>

    <section class="testimonials" id="testimonials">
        <div class="container">
            <h2>What Our Users Say</h2>
            <div class="testimonial-grid">
                <div class="testimonial-card">
                    <p class="testimonial-text">This resume builder helped me land my dream job! The templates are professional and the process was so easy.</p>
                    <p class="testimonial-author">- Sarah Johnson, Marketing Manager</p>
                </div>
                <div class="testimonial-card">
                    <p class="testimonial-text">I was able to create a polished resume in under 15 minutes. The download feature works perfectly.</p>
                    <p class="testimonial-author">- Michael Chen, Software Engineer</p>
                </div>
                <div class="testimonial-card">
                    <p class="testimonial-text">As a recent graduate, I didn't know how to structure my resume. This tool guided me through the process.</p>
                    <p class="testimonial-author">- David Wilson, Recent Graduate</p>
                </div>
            </div>
        </div>
    </section>

    <section class="feedback-section" id="feedback">
        <div class="container">
            <h2>Share Your Feedback</h2>
            <div class="feedback-form">
                <div class="form-group">
                    <label for="feedbackName">Your Name</label>
                    <input type="text" id="feedbackName" placeholder="Your name">
                </div>
                
                <div class="form-group">
                    <label for="feedbackEmail">Email (optional)</label>
                    <input type="email" id="feedbackEmail" placeholder="your.email@example.com">
                </div>
                
                <div class="form-group">
                    <label>How would you rate our resume builder?</label>
                    <div class="rating-container">
                        <input type="radio" id="star5" name="rating" value="5" class="rating-input">
                        <label for="star5" class="rating-label">★</label>
                        <input type="radio" id="star4" name="rating" value="4" class="rating-input">
                        <label for="star4" class="rating-label">★</label>
                        <input type="radio" id="star3" name="rating" value="3" class="rating-input">
                        <label for="star3" class="rating-label">★</label>
                        <input type="radio" id="star2" name="rating" value="2" class="rating-input">
                        <label for="star2" class="rating-label">★</label>
                        <input type="radio" id="star1" name="rating" value="1" class="rating-input">
                        <label for="star1" class="rating-label">★</label>
                    </div>
                </div>
                
                <div class="form-group">
                    <label for="feedbackMessage">Your Feedback</label>
                    <textarea id="feedbackMessage" placeholder="What did you like or what can we improve?"></textarea>
                </div>
                
                <button type="button" class="cta-button" id="submitFeedback">
                    <i class="fas fa-paper-plane"></i> Submit Feedback
                </button>
            </div>
        </div>
    </section>

    <!-- Footer Ad Space -->
    <div class="container">
        <div class="ad-container">
            <div class="ad-label">Advertisement</div>
            <!-- Google AdSense Ad Unit -->
            <script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-pub-XXXXXXXXXXXXXXXX"
                crossorigin="anonymous"></script>
            <!-- Resume Builder Footer Banner -->
            <ins class="adsbygoogle"
                style="display:block"
                data-ad-client="ca-pub-XXXXXXXXXXXXXXXX"
                data-ad-slot="XXXXXXXXXX"
                data-ad-format="auto"
                data-full-width-responsive="true"></ins>
            <script>
                (adsbygoogle = window.adsbygoogle || []).push({});
            </script>
        </div>
    </div>

    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="logo">
                   
