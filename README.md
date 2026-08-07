<!DOCTYPE html>
<html lang="mr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Apex English School & Junior College, Pangri</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --navy-dark: #001f3f;
            --navy-header: #001933;
            --gold-accent: #f39c12;
            --gold-light: #f1c40f;
            --green-whatsapp: #25d366;
            --ba-orange: #d35400;
            --ma-purple: #4a235a;
            --msw-green: #1e8449;
            --bg-light: #f4f6f9;
        }

        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; }
        body { background-color: var(--bg-light); color: #333; line-height: 1.6; }

        /* Top Navigation */
        .top-nav { background-color: var(--navy-header); color: #fff; padding: 15px 5%; display: flex; justify-content: space-between; align-items: center; flex-wrap: wrap; border-bottom: 2px solid var(--gold-accent); }
        .logo-area { display: flex; align-items: center; gap: 12px; }
        .logo-icon { background: var(--gold-accent); color: var(--navy-dark); width: 45px; height: 45px; border-radius: 50%; display: flex; align-items: center; justify-content: center; font-size: 1.5rem; font-weight: bold; }
        .logo-text h1 { font-size: 1.2rem; text-transform: uppercase; letter-spacing: 1px; color: #fff; }
        .logo-text p { font-size: 0.8rem; color: #ccc; }

        .nav-menu { display: flex; gap: 20px; list-style: none; }
        .nav-menu a { color: #fff; text-decoration: none; font-weight: 600; font-size: 0.95rem; text-transform: uppercase; transition: 0.3s; padding-bottom: 5px; }
        .nav-menu a:hover, .nav-menu a.active { color: var(--gold-light); border-bottom: 2px solid var(--gold-light); }

        /* Hero Front Page Banner Section */
        .hero-section { background: linear-gradient(135deg, #001f3f 0%, #003366 100%); color: #fff; padding: 40px 5%; display: flex; align-items: center; justify-content: space-between; flex-wrap: wrap; gap: 30px; }
        .hero-content { flex: 1; min-width: 300px; }
        .hero-title { font-size: 2.8rem; font-weight: 900; color: #fff; line-height: 1.1; margin-bottom: 10px; }
        .hero-year { color: var(--gold-light); font-size: 3rem; }
        .hero-subtitle { font-size: 1.8rem; font-weight: 800; color: #fff; margin-bottom: 15px; letter-spacing: 1px; }
        .hero-tag { background: var(--gold-accent); color: #000; display: inline-block; padding: 8px 20px; font-weight: bold; border-radius: 20px; font-size: 1.1rem; margin-bottom: 15px; }
        .hero-desc { font-size: 1.1rem; margin-bottom: 25px; opacity: 0.9; }

        /* Action Buttons */
        .hero-btns { display: flex; gap: 15px; flex-wrap: wrap; }
        .btn-call { background: var(--navy-header); color: #fff; border: 1px solid #fff; padding: 12px 25px; border-radius: 30px; text-decoration: none; font-weight: bold; display: inline-flex; align-items: center; gap: 8px; transition: 0.3s; }
        .btn-call:hover { background: #fff; color: var(--navy-dark); }
        
        .btn-wa { background: var(--green-whatsapp); color: #fff; padding: 12px 25px; border-radius: 30px; text-decoration: none; font-weight: bold; display: inline-flex; align-items: center; gap: 8px; transition: 0.3s; box-shadow: 0 4px 10px rgba(37, 211, 102, 0.3); }
        .btn-wa:hover { background: #1ebc57; transform: translateY(-2px); }

        .hero-image-box { flex: 1; min-width: 300px; text-align: center; }
        .building-card { background: #fff; color: var(--navy-dark); padding: 25px; border-radius: 15px; box-shadow: 0 10px 25px rgba(0,0,0,0.3); border: 3px solid var(--gold-accent); display: inline-block; width: 100%; max-width: 450px; }

        /* Container */
        .container { max-width: 1200px; margin: 40px auto; padding: 0 15px; }

        /* Courses Grid */
        .courses-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(320px, 1fr)); gap: 25px; margin-bottom: 40px; }
        .course-card { background: #fff; border-radius: 15px; overflow: hidden; box-shadow: 0 5px 15px rgba(0,0,0,0.08); border: 1px solid #e0e0e0; display: flex; flex-direction: column; justify-content: space-between; }
        
        .card-header { text-align: center; padding: 20px; }
        .card-header.ba { color: var(--ba-orange); border-bottom: 2px solid var(--ba-orange); }
        .card-header.ma { color: var(--ma-purple); border-bottom: 2px solid var(--ma-purple); }
        .card-header.msw { color: var(--msw-green); border-bottom: 2px solid var(--msw-green); }
        .card-header h2 { font-size: 2.5rem; font-weight: 900; }

        .admission-tag { display: block; text-align: center; color: #fff; padding: 6px; font-weight: bold; font-size: 0.9rem; }
        .ba-tag { background: var(--ba-orange); }
        .ma-tag { background: var(--ma-purple); }
        .msw-tag { background: var(--msw-green); }

        .card-body { padding: 20px; flex-grow: 1; }
        .card-body ul { list-style: none; }
        .card-body ul li { margin-bottom: 8px; position: relative; padding-left: 20px; font-size: 0.95rem; }
        .card-body ul li::before { content: "●"; position: absolute; left: 0; }
        .ba-list li::before { color: var(--ba-orange); }
        .ma-list li::before { color: var(--ma-purple); }
        .msw-list li::before { color: var(--msw-green); }

        .card-footer-banner { text-align: center; color: #fff; padding: 10px; font-weight: bold; font-size: 1rem; }
        .ba-footer { background: var(--ba-orange); }
        .ma-footer { background: var(--ma-purple); }
        .msw-footer { background: var(--msw-green); }

        /* Bottom Contact Section */
        .bottom-section { display: grid; grid-template-columns: repeat(auto-fit, minmax(320px, 1fr)); gap: 25px; background: var(--navy-dark); color: #fff; padding: 30px; border-radius: 15px; margin-bottom: 30px; }
        .why-us h3, .contact-us h3 { color: var(--gold-light); font-size: 1.5rem; margin-bottom: 20px; }
        .why-us-list { list-style: none; }
        .why-us-list li { margin-bottom: 12px; display: flex; align-items: center; gap: 10px; }
        .why-us-list i { color: var(--gold-light); }

        .contact-card { background: #fff; color: #000; padding: 12px 20px; border-radius: 10px; margin-bottom: 12px; display: flex; align-items: center; gap: 15px; }
        .contact-icon { background: var(--navy-dark); color: #fff; width: 40px; height: 40px; border-radius: 50%; display: flex; align-items: center; justify-content: center; font-size: 1.2rem; }
        .contact-info p { font-size: 1.1rem; font-weight: bold; color: var(--navy-dark); }

        .cta-banner { background: var(--gold-accent); color: #000; text-align: center; padding: 15px; border-radius: 10px; font-weight: bold; font-size: 1.2rem; }

        footer { background: var(--navy-header); color: #ccc; text-align: center; padding: 20px; font-size: 0.9rem; }
        .footer-links { display: flex; justify-content: center; gap: 20px; margin-bottom: 10px; }
        .footer-links a { color: #ccc; text-decoration: none; }
    </style>
</head>
<body>

    <!-- Header Navigation -->
    <nav class="top-nav">
        <div class="logo-area">
            <div class="logo-icon">A</div>
            <div class="logo-text">
                <h1>Apex English School</h1>
                <p>& Junior College, Pangri</p>
            </div>
        </div>
        <ul class="nav-menu">
            <li><a href="#" class="active">Home</a></li>
            <li><a href="#courses">About Us</a></li>
            <li><a href="#courses">Courses</a></li>
            <li><a href="#why-us">Gallery</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>

    <!-- Front Page Hero Banner -->
    <section class="hero-section">
        <div class="hero-content">
            <h1 class="hero-title">ADMISSION <br><span class="hero-year">2026-27</span></h1>
            <div class="hero-subtitle">OPEN NOW!</div>
            <div class="hero-tag">Build Your Future With Us</div>
            <p class="hero-desc">Quality Education, Bright Future and Successful Career.</p>
            
            <div class="hero-btns">
                <a href="tel:8999751028" class="btn-call"><i class="fa-solid fa-phone"></i> Call Now</a>
                <!-- Direct WhatsApp Link to 8999751028 -->
                <a href="https://wa.me/918999751028?text=नमस्कार,%20मला%20प्रवेशाबद्दल%20माहिती%20हवी%20आहे." target="_blank" class="btn-wa">
                    <i class="fa-brands fa-whatsapp"></i> WhatsApp
                </a>
            </div>
        </div>

        <div class="hero-image-box">
            <div class="building-card">
                <h2 style="color: #001f3f; font-size: 1.6rem; font-weight: 900;">APEX ENGLISH SCHOOL</h2>
                <p style="color: #666; font-weight: bold; margin-bottom: 5px;">& JUNIOR COLLEGE, PANGRI</p>
                <p style="font-size: 0.85rem; color: #888;">(Tq. Sillod, Dist. Chhatrapati Sambhajinagar)</p>
                
                <div style="margin-top: 20px; background: #8b0000; color: #fff; padding: 12px; border-radius: 8px; font-weight: bold; font-size: 1.1rem;">
                    ADMISSION OPEN 2026-27
                </div>
            </div>
        </div>
    </section>

    <div class="container">

        <!-- Courses Section -->
        <div id="courses" class="courses-grid">
            
            <!-- B.A. Card -->
            <div class="course-card">
                <div>
                    <div class="card-header ba">
                        <h2>B.A.</h2>
                        <p style="font-size: 1.1rem; font-weight: bold;">प्रशासकीय सेवा</p>
                        <span style="font-size: 0.85rem; color: #666;">(Bachelor of Arts)</span>
                    </div>
                    <div class="admission-tag ba-tag">ADMISSION OPEN 2026-27</div>
                    <div class="card-body">
                        <h4 style="color: var(--ba-orange); margin-bottom: 10px;">विशेष वैशिष्ट्ये</h4>
                        <ul class="ba-list">
                            <li>प्रशासकीय सेवांची तयारी</li>
                            <li>अनुभवी व तज्ज्ञ शिक्षकवर्ग</li>
                            <li>गुणवत्तापूर्ण शिक्षण व्यवस्था</li>
                            <li>सर्वांगीण व्यक्तिमत्त्व विकास</li>
                        </ul>
                    </div>
                </div>
                <div class="card-footer-banner ba-footer">ज्ञान हाच खरा खजिना !</div>
            </div>

            <!-- M.A. Card -->
            <div class="course-card">
                <div>
                    <div class="card-header ma">
                        <h2>M.A.</h2>
                        <p style="font-size: 1.1rem; font-weight: bold;">Public Administration</p>
                    </div>
                    <div class="admission-tag ma-tag">ADMISSION OPEN 2026-27</div>
                    <div class="card-body">
                        <h4 style="color: var(--ma-purple); margin-bottom: 10px;">Our Features</h4>
                        <ul class="ma-list">
                            <li>Experienced Faculty</li>
                            <li>Quality Education</li>
                            <li>Career Oriented Study</li>
                            <li>Personality Development</li>
                        </ul>
                    </div>
                </div>
                <div class="card-footer-banner ma-footer">Make A Better Future Through Better Education</div>
            </div>

            <!-- MSW Card -->
            <div class="course-card">
                <div>
                    <div class="card-header msw">
                        <h2>MSW</h2>
                        <p style="font-size: 1.1rem; font-weight: bold;">Master of Social Work</p>
                    </div>
                    <div class="admission-tag msw-tag">ADMISSION OPEN 2026-27</div>
                    <div class="card-body">
                        <h4 style="color: var(--msw-green); margin-bottom: 10px;">Our Highlights</h4>
                        <ul class="msw-list">
                            <li>Experienced Faculty</li>
                            <li>Practical Based Learning</li>
                            <li>Field Work & Project</li>
                            <li>Career Opportunities</li>
                        </ul>
                    </div>
                </div>
                <div class="card-footer-banner msw-footer">Empower People, Change the World</div>
            </div>

        </div>

        <!-- Bottom Contact & Why Choose Us -->
        <div id="why-us" class="bottom-section">
            <div class="why-us">
                <h3><i class="fa-solid fa-graduation-cap"></i> Why Choose Us?</h3>
                <ul class="why-us-list">
                    <li><i class="fa-regular fa-circle-check"></i> Experienced & Dedicated Faculty</li>
                    <li><i class="fa-regular fa-circle-check"></i> Modern Learning Environment</li>
                    <li><i class="fa-regular fa-circle-check"></i> Smart Classrooms & ICT Facilities</li>
                    <li><i class="fa-regular fa-circle-check"></i> Focus on Personality Development</li>
                    <li><i class="fa-regular fa-circle-check"></i> Career Guidance & Support</li>
                    <li><i class="fa-regular fa-circle-check"></i> Safe & Friendly Campus</li>
                </ul>
            </div>

            <div id="contact" class="contact-us">
                <h3><i class="fa-solid fa-address-book"></i> Contact Us</h3>
                
                <div class="contact-card">
                    <div class="contact-icon"><i class="fa-solid fa-phone"></i></div>
                    <div class="contact-info">
                        <h4>Digvijay Jadhav Sir</h4>
                        <p><a href="tel:7350731369" style="text-decoration:none; color:inherit;">7350731369</a></p>
                    </div>
                </div>

                <div class="contact-card">
                    <div class="contact-icon"><i class="fa-solid fa-phone"></i></div>
                    <div class="contact-info">
                        <h4>Pavan Jadhav Sir</h4>
                        <p><a href="tel:7218933938" style="text-decoration:none; color:inherit;">7218933938</a></p>
                    </div>
                </div>

                <div class="contact-card">
                    <div class="contact-icon"><i class="fa-solid fa-phone"></i></div>
                    <div class="contact-info">
                        <h4>Kiran Jadhav Sir</h4>
                        <p><a href="tel:8999751028" style="text-decoration:none; color:inherit;">8999751028</a></p>
                    </div>
                </div>
            </div>
        </div>

        <div class="cta-banner">
            Take the First Step Towards a Successful Future with Apex!
        </div>

    </div>

    <!-- Footer -->
    <footer>
        <div class="footer-links">
            <a href="#">HOME</a> | 
            <a href="#">ABOUT US</a> | 
            <a href="#">COURSES</a> | 
            <a href="#">GALLERY</a> | 
            <a href="#">CONTACT</a>
        </div>
        <p>&copy; 2026-27 Apex English School & Junior College, Pangri. All Rights Reserved.</p>
    </footer>

</body>
</html>
