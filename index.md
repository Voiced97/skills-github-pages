
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Visual-Auditory Perception of Plosives</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: #333;
            overflow: hidden;
        }
        
        .presentation-container {
            width: 100vw;
            height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        
        .slide {
            width: 90%;
            max-width: 1200px;
            height: 80vh;
            background: white;
            border-radius: 20px;
            box-shadow: 0 20px 40px rgba(0,0,0,0.1);
            padding: 60px;
            display: none;
            flex-direction: column;
            justify-content: center;
            position: relative;
        }
        
        .slide.active {
            display: flex;
        }
        
        .slide h1 {
            font-size: 2.8em;
            color: #2c3e50;
            text-align: center;
            margin-bottom: 30px;
            border-bottom: 4px solid #3498db;
            padding-bottom: 20px;
        }
        
        .slide h2 {
            font-size: 2.2em;
            color: #34495e;
            margin-bottom: 25px;
            text-align: center;
        }
        
        .slide h3 {
            font-size: 1.8em;
            color: #2980b9;
            margin-bottom: 20px;
        }
        
        .slide p, .slide li {
            font-size: 1.3em;
            line-height: 1.6;
            margin-bottom: 15px;
            color: #444;
        }
        
        .slide ul {
            margin-left: 30px;
            margin-bottom: 25px;
        }
        
        .highlight {
            background: linear-gradient(120deg, #a8edea 0%, #fed6e3 100%);
            padding: 3px 8px;
            border-radius: 5px;
            font-weight: bold;
        }
        
        .definition-box {
            background: #f8f9fa;
            border-left: 5px solid #3498db;
            padding: 20px;
            margin: 20px 0;
            border-radius: 5px;
        }
        
        .research-gap {
            background: linear-gradient(135deg, #ffeaa7 0%, #fab1a0 100%);
            padding: 25px;
            border-radius: 15px;
            margin: 20px 0;
            text-align: center;
        }
        
        .navigation {
            position: fixed;
            bottom: 30px;
            left: 50%;
            transform: translateX(-50%);
            display: flex;
            gap: 15px;
        }
        
        .nav-btn {
            padding: 12px 25px;
            background: #3498db;
            color: white;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            font-size: 1.1em;
            transition: all 0.3s ease;
        }
        
        .nav-btn:hover {
            background: #2980b9;
            transform: translateY(-2px);
        }
        
        .slide-counter {
            position: absolute;
            top: 20px;
            right: 30px;
            background: #34495e;
            color: white;
            padding: 8px 15px;
            border-radius: 20px;
            font-size: 1.1em;
        }
        
        .references {
            font-size: 1em;
            color: #666;
            margin-top: 20px;
        }
        
        .method-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 30px;
            margin-top: 20px;
        }
        
        .method-card {
            background: #ecf0f1;
            padding: 20px;
            border-radius: 10px;
            border-left: 4px solid #e74c3c;
        }
    </style>
</head>
<body>
    <div class="presentation-container">
        <!-- Slide 1: Title -->
        <div class="slide active">
            <div class="slide-counter">1 / 8</div>
            <h1>Visual-Auditory Perception of Plosives:</h1>
            <h2 style="color: #7f8c8d; margin-top: 20px;">Investigating Cross-modal Effects on Voicing Perception in Japanese</h2>
            <div style="text-align: center; margin-top: 50px; font-size: 1.4em; color: #2c3e50;">
                <p><strong>Research Focus:</strong> How visual cues influence plosive voicing perception</p>
            </div>
        </div>

        <!-- Slide 2: What are Plosives? -->
        <div class="slide">
            <div class="slide-counter">2 / 8</div>
            <h2>What are Plosives?</h2>
            <div class="definition-box">
                <h3>Definition:</h3>
                <p><span class="highlight">Plosives</span> (also called stops) are consonant sounds produced by completely blocking airflow in the vocal tract, then releasing it suddenly.</p>
            </div>
            
            <h3>Examples in Different Languages:</h3>
            <ul>
                <li><strong>English:</strong> /p/, /b/, /t/, /d/, /k/, /g/</li>
                <li><strong>Japanese:</strong> /p/, /b/, /t/, /d/, /k/, /g/</li>
                <li><strong>Key Feature:</strong> <span class="highlight">Voicing distinction</span> (voiced vs. voiceless)</li>
            </ul>
            
            <div class="references">
                <p><strong>Reference:</strong> Ladefoged, P., & Johnson, K. (2014). <em>A Course in Phonetics</em>. Cengage Learning.</p>
            </div>
        </div>

        <!-- Slide 3: VOT -->
        <div class="slide">
            <div class="slide-counter">3 / 8</div>
            <h2>Voice Onset Time (VOT)</h2>
            <div class="definition-box">
                <h3>Abramson & Lisker (1964) Definition:</h3>
                <p><span class="highlight">VOT</span> is the time interval between the release of a stop closure and the onset of vocal fold vibration.</p>
            </div>
            
            <h3>VOT Categories:</h3>
            <ul>
                <li><strong>Negative VOT:</strong> Voicing starts before release (pre-voiced)</li>
                <li><strong>Short-lag VOT:</strong> Voicing starts shortly after release (0-30ms)</li>
                <li><strong>Long-lag VOT:</strong> Voicing starts long after release (30ms+)</li>
            </ul>
            
            <p style="margin-top: 25px;"><span class="highlight">Significance:</span> VOT is considered a <strong>robust acoustic cue</strong> for voicing distinction across languages.</p>
            
            <div class="references">
                <p><strong>Key Reference:</strong> Abramson, A. S., & Lisker, L. (1964). A cross-language study of voicing in initial stops. <em>Word</em>, 20(3), 384-422.</p>
            </div>
        </div>

        <!-- Slide 4: Japanese Specificity -->
        <div class="slide">
            <div class="slide-counter">4 / 8</div>
            <h2>Japanese: Beyond VOT</h2>
            
            <div class="definition-box">
                <h3>Japanese Complexity:</h3>
                <p>Research suggests that Japanese speakers rely on <span class="highlight">multiple acoustic cues</span> beyond VOT for voicing perception.</p>
            </div>
            
            <h3>Additional Cues in Japanese:</h3>
            <ul>
                <li><strong>F0 (Fundamental frequency)</strong> of following vowel</li>
                <li><strong>Vowel duration</strong></li>
                <li><strong>Spectral characteristics</strong></li>
                <li><strong>Closure duration</strong></li>
            </ul>
            
            <p style="margin-top: 25px;"><span class="highlight">Implication:</span> Japanese voicing perception is more complex than VOT-based models suggest.</p>
            
            <div class="references">
                <p><strong>References:</strong><br>
                • Shimizu, K. (1996). A cross-language study of voicing contrasts of stop consonants in Asian languages. <em>Seibido</em>.<br>
                • Homma, Y. (1981). Durational relationship between Japanese stops and vowels. <em>Journal of Phonetics</em>, 9(3), 273-281.</p>
            </div>
        </div>

        <!-- Slide 5: Visual-Auditory Perception -->
        <div class="slide">
            <div class="slide-counter">5 / 8</div>
            <h2>Visual-Auditory Speech Perception</h2>
            
            <h3>Traditional View:</h3>
            <p>Speech perception was traditionally considered <span class="highlight">primarily auditory</span>, with acoustic cues dominating perception.</p>
            
            <div class="definition-box">
                <h3>McGurk Effect (1976):</h3>
                <p>Demonstrated that <span class="highlight">visual information</span> (lip movements) can significantly influence what we <strong>hear</strong>.</p>
                <ul style="margin-top: 15px;">
                    <li>Visual /ga/ + Auditory /ba/ → Perceived /da/</li>
                    <li>Shows <strong>mandatory integration</strong> of visual-auditory information</li>
                </ul>
            </div>
            
            <h3>Modern Understanding:</h3>
            <p><span class="highlight">Multimodal integration</span> is fundamental to speech perception - humans naturally combine visual and auditory cues.</p>
            
            <div class="references">
                <p><strong>Key Reference:</strong> McGurk, H., & MacDonald, J. (1976). Hearing lips and seeing voices. <em>Nature</em>, 264(5588), 746-748.</p>
            </div>
        </div>

        <!-- Slide 6: Research Gap -->
        <div class="slide">
            <div class="slide-counter">6 / 8</div>
            <h2>Research Gap</h2>
            
            <div class="research-gap">
                <h3>🔍 Identified Gap</h3>
                <p><strong>Limited research on visual effects on plosive voicing perception in Japanese</strong></p>
            </div>
            
            <h3>What We Know:</h3>
            <ul>
                <li>McGurk effect exists for various speech sounds</li>
                <li>Japanese has complex voicing cue system</li>
                <li>Visual cues affect place of articulation perception</li>
            </ul>
            
            <h3>What's Missing:</h3>
            <ul>
                <li><span class="highlight">Specific investigation</span> of visual effects on <strong>voicing perception</strong></li>
                <li><strong>Japanese-specific</strong> studies on multimodal plosive perception</li>
                <li>Understanding of <strong>lip movement cues</strong> for voicing distinction</li>
            </ul>
            
            <div style="margin-top: 25px; padding: 15px; background: #d5f4e6; border-radius: 10px;">
                <strong>Research Question:</strong> How do visual cues (lip movements) influence plosive voicing perception in Japanese?
            </div>
        </div>

        <!-- Slide 7: Methodology -->
        <div class="slide">
            <div class="slide-counter">7 / 8</div>
            <h2>Proposed Methodology</h2>
            
            <h3>Experimental Design:</h3>
            <div class="method-grid">
                <div class="method-card">
                    <h4>🎯 Stimulus Manipulation</h4>
                    <ul>
                        <li>Modify/weaken acoustic cues (VOT manipulation)</li>
                        <li>Create ambiguous voicing stimuli</li>
                        <li>Amplify potential visual effects</li>
                    </ul>
                </div>
                
                <div class="method-card">
                    <h4>👁️ Conditions</h4>
                    <ul>
                        <li><strong>Auditory-only:</strong> Audio stimuli</li>
                        <li><strong>Visual-only:</strong> Lip movements</li>
                        <li><strong>Audiovisual:</strong> Combined stimuli</li>
                    </ul>
                </div>
            </div>
            
            <h3>Quantitative Approach:</h3>
            <ul>
                <li><strong>Large sample size</strong> of Japanese speakers</li>
                <li><strong>Perceptual categorization task</strong> (voiced/voiceless judgments)</li>
                <li><strong>Statistical analysis</strong> of visual influence on perception</li>
                <li><strong>Reaction time measurements</strong></li>
            </ul>
            
            <div class="definition-box">
                <strong>Hypothesis:</strong> Visual cues will show measurable influence on voicing perception, especially for acoustically ambiguous stimuli.
            </div>
        </div>

        <!-- Slide 8: Expected Outcomes -->
        <div class="slide">
            <div class="slide-counter">8 / 8</div>
            <h2>Expected Outcomes & Significance</h2>
            
            <h3>Expected Results:</h3>
            <ul>
                <li><span class="highlight">Quantifiable visual influence</span> on voicing perception</li>
                <li><strong>Individual differences</strong> in visual-auditory integration</li>
                <li><strong>Stimulus-specific effects</strong> (different plosives may show varying visual influence)</li>
            </ul>
            
            <h3>Theoretical Contributions:</h3>
            <ul>
                <li><strong>Expand understanding</strong> of Japanese speech perception</li>
                <li><strong>Contribute to multimodal perception theory</strong></li>
                <li><strong>Bridge phonetics and psycholinguistics</strong></li>
            </ul>
            
            <h3>Practical Applications:</h3>
            <ul>
                <li><strong>Language learning</strong> and pronunciation training</li>
                <li><strong>Speech therapy</strong> approaches</li>
                <li><strong>Hearing aid technology</strong> development</li>
            </ul>
            
            <div style="text-align: center; margin-top: 30px; padding: 20px; background: linear-gradient(135deg, #74b9ff, #0984e3); color: white; border-radius: 15px;">
                <h3>Thank You for Your Attention!</h3>
                <p>Questions & Discussion Welcome</p>
            </div>
        </div>
    </div>

    <div class="navigation">
        <button class="nav-btn" onclick="previousSlide()">← Previous</button>
        <button class="nav-btn" onclick="nextSlide()">Next →</button>
    </div>

    <script>
        let currentSlide = 0;
        const slides = document.querySelectorAll('.slide');
        const totalSlides = slides.length;

        function showSlide(n) {
            slides[currentSlide].classList.remove('active');
            currentSlide = (n + totalSlides) % totalSlides;
            slides[currentSlide].classList.add('active');
        }

        function nextSlide() {
            showSlide(currentSlide + 1);
        }

        function previousSlide() {
            showSlide(currentSlide - 1);
        }

        // Keyboard navigation
        document.addEventListener('keydown', function(e) {
            if (e.key === 'ArrowRight' || e.key === ' ') {
                nextSlide();
            } else if (e.key === 'ArrowLeft') {
                previousSlide();
            }
        });

        // Auto-advance for presentation mode (optional)
        // setInterval(nextSlide, 45000); // Uncomment for 45-second auto-advance
    </script>
</body>
</html>
