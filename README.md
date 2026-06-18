# Anatomy-
Question Generator
[discussion-spinner.html](https://github.com/user-attachments/files/29115461/discussion-spinner.html)
<!DOCTYPE html PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">
<html>
<head>
  <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
  <meta http-equiv="Content-Style-Type" content="text/css">
  <title></title>
  <meta name="Generator" content="Cocoa HTML Writer">
  <meta name="CocoaVersion" content="2575.7">
  <style type="text/css">
    p.p1 {margin: 0.0px 0.0px 0.0px 0.0px; font: 12.0px Helvetica}
    p.p2 {margin: 0.0px 0.0px 0.0px 0.0px; font: 12.0px Helvetica; min-height: 14.0px}
  </style>
</head>
<body>
<p class="p1">&lt;!DOCTYPE html&gt;</p>
<p class="p1">&lt;html lang="en"&gt;</p>
<p class="p1">&lt;head&gt;</p>
<p class="p1"><span class="Apple-converted-space">  </span>&lt;meta charset="UTF-8"&gt;</p>
<p class="p1"><span class="Apple-converted-space">  </span>&lt;meta name="viewport" content="width=device-width, initial-scale=1.0"&gt;</p>
<p class="p1"><span class="Apple-converted-space">  </span>&lt;title&gt;Discussion Question Spinner&lt;/title&gt;</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">  </span>&lt;style&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>body {</p>
<p class="p1"><span class="Apple-converted-space">      </span>font-family: Arial, Helvetica, sans-serif;</p>
<p class="p1"><span class="Apple-converted-space">      </span>text-align: center;</p>
<p class="p1"><span class="Apple-converted-space">      </span>padding: 20px;</p>
<p class="p1"><span class="Apple-converted-space">      </span>color: #333;</p>
<p class="p1"><span class="Apple-converted-space">      </span>background-color: #f8f9fa;</p>
<p class="p1"><span class="Apple-converted-space">    </span>}</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">    </span>h2 {</p>
<p class="p1"><span class="Apple-converted-space">      </span>margin-bottom: 10px;</p>
<p class="p1"><span class="Apple-converted-space">    </span>}</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">    </span>p.instructions {</p>
<p class="p1"><span class="Apple-converted-space">      </span>max-width: 700px;</p>
<p class="p1"><span class="Apple-converted-space">      </span>margin: 0 auto 20px;</p>
<p class="p1"><span class="Apple-converted-space">      </span>line-height: 1.5;</p>
<p class="p1"><span class="Apple-converted-space">    </span>}</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">    </span>#pointer {</p>
<p class="p1"><span class="Apple-converted-space">      </span>width: 0;</p>
<p class="p1"><span class="Apple-converted-space">      </span>height: 0;</p>
<p class="p1"><span class="Apple-converted-space">      </span>border-left: 20px solid transparent;</p>
<p class="p1"><span class="Apple-converted-space">      </span>border-right: 20px solid transparent;</p>
<p class="p1"><span class="Apple-converted-space">      </span>border-top: 35px solid #333;</p>
<p class="p1"><span class="Apple-converted-space">      </span>margin: 0 auto -5px;</p>
<p class="p1"><span class="Apple-converted-space">      </span>z-index: 2;</p>
<p class="p1"><span class="Apple-converted-space">      </span>position: relative;</p>
<p class="p1"><span class="Apple-converted-space">    </span>}</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">    </span>#wheel-container {</p>
<p class="p1"><span class="Apple-converted-space">      </span>position: relative;</p>
<p class="p1"><span class="Apple-converted-space">      </span>width: 320px;</p>
<p class="p1"><span class="Apple-converted-space">      </span>height: 320px;</p>
<p class="p1"><span class="Apple-converted-space">      </span>margin: 0 auto 25px;</p>
<p class="p1"><span class="Apple-converted-space">    </span>}</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">    </span>#wheel {</p>
<p class="p1"><span class="Apple-converted-space">      </span>width: 320px;</p>
<p class="p1"><span class="Apple-converted-space">      </span>height: 320px;</p>
<p class="p1"><span class="Apple-converted-space">      </span>border-radius: 50%;</p>
<p class="p1"><span class="Apple-converted-space">      </span>border: 8px solid #333;</p>
<p class="p1"><span class="Apple-converted-space">      </span>transition: transform 4s ease-out;</p>
<p class="p1"><span class="Apple-converted-space">      </span>background: conic-gradient(</p>
<p class="p1"><span class="Apple-converted-space">        </span>#f7c59f 0deg 36deg,</p>
<p class="p1"><span class="Apple-converted-space">        </span>#b7d7a8 36deg 72deg,</p>
<p class="p1"><span class="Apple-converted-space">        </span>#a2c4c9 72deg 108deg,</p>
<p class="p1"><span class="Apple-converted-space">        </span>#d9a5b3 108deg 144deg,</p>
<p class="p1"><span class="Apple-converted-space">        </span>#ffe599 144deg 180deg,</p>
<p class="p1"><span class="Apple-converted-space">        </span>#c9daf8 180deg 216deg,</p>
<p class="p1"><span class="Apple-converted-space">        </span>#d5a6bd 216deg 252deg,</p>
<p class="p1"><span class="Apple-converted-space">        </span>#b6d7a8 252deg 288deg,</p>
<p class="p1"><span class="Apple-converted-space">        </span>#f4cccc 288deg 324deg,</p>
<p class="p1"><span class="Apple-converted-space">        </span>#d9ead3 324deg 360deg</p>
<p class="p1"><span class="Apple-converted-space">      </span>);</p>
<p class="p1"><span class="Apple-converted-space">    </span>}</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">    </span>button {</p>
<p class="p1"><span class="Apple-converted-space">      </span>background-color: #2c3e50;</p>
<p class="p1"><span class="Apple-converted-space">      </span>color: white;</p>
<p class="p1"><span class="Apple-converted-space">      </span>border: none;</p>
<p class="p1"><span class="Apple-converted-space">      </span>border-radius: 8px;</p>
<p class="p1"><span class="Apple-converted-space">      </span>padding: 12px 24px;</p>
<p class="p1"><span class="Apple-converted-space">      </span>font-size: 18px;</p>
<p class="p1"><span class="Apple-converted-space">      </span>cursor: pointer;</p>
<p class="p1"><span class="Apple-converted-space">      </span>margin-bottom: 20px;</p>
<p class="p1"><span class="Apple-converted-space">    </span>}</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">    </span>button:hover {</p>
<p class="p1"><span class="Apple-converted-space">      </span>background-color: #1f2d3a;</p>
<p class="p1"><span class="Apple-converted-space">    </span>}</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">    </span>#result {</p>
<p class="p1"><span class="Apple-converted-space">      </span>max-width: 800px;</p>
<p class="p1"><span class="Apple-converted-space">      </span>margin: 0 auto;</p>
<p class="p1"><span class="Apple-converted-space">      </span>padding: 16px;</p>
<p class="p1"><span class="Apple-converted-space">      </span>min-height: 60px;</p>
<p class="p1"><span class="Apple-converted-space">      </span>font-size: 1.2rem;</p>
<p class="p1"><span class="Apple-converted-space">      </span>font-weight: bold;</p>
<p class="p1"><span class="Apple-converted-space">      </span>background-color: white;</p>
<p class="p1"><span class="Apple-converted-space">      </span>border-radius: 10px;</p>
<p class="p1"><span class="Apple-converted-space">      </span>border: 2px solid #ddd;</p>
<p class="p1"><span class="Apple-converted-space">    </span>}</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">    </span>.followup {</p>
<p class="p1"><span class="Apple-converted-space">      </span>margin-top: 20px;</p>
<p class="p1"><span class="Apple-converted-space">      </span>font-size: 1rem;</p>
<p class="p1"><span class="Apple-converted-space">    </span>}</p>
<p class="p1"><span class="Apple-converted-space">  </span>&lt;/style&gt;</p>
<p class="p1">&lt;/head&gt;</p>
<p class="p2"><br></p>
<p class="p1">&lt;body&gt;</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">  </span>&lt;h2&gt;Discussion Question Spinner&lt;/h2&gt;</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">  </span>&lt;p class="instructions"&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>Click the button to spin the wheel. Answer the question you receive in your discussion post.</p>
<p class="p1"><span class="Apple-converted-space">  </span>&lt;/p&gt;</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">  </span>&lt;div id="pointer"&gt;&lt;/div&gt;</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">  </span>&lt;div id="wheel-container"&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;div id="wheel"&gt;&lt;/div&gt;</p>
<p class="p1"><span class="Apple-converted-space">  </span>&lt;/div&gt;</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">  </span>&lt;button onclick="spinWheel()"&gt;Spin the Wheel&lt;/button&gt;</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">  </span>&lt;div id="result"&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>Your question will appear here.</p>
<p class="p1"><span class="Apple-converted-space">  </span>&lt;/div&gt;</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">  </span>&lt;p class="followup"&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>&lt;strong&gt;After posting your response, reply to at least one classmate.&lt;/strong&gt;</p>
<p class="p1"><span class="Apple-converted-space">  </span>&lt;/p&gt;</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">  </span>&lt;script&gt;</p>
<p class="p1"><span class="Apple-converted-space">    </span>const questions = [</p>
<p class="p1"><span class="Apple-converted-space">      </span>"What topic could you give a TED Talk on with no preparation time?",</p>
<p class="p1"><span class="Apple-converted-space">      </span>"What is your favorite dinosaur? Why?",</p>
<p class="p1"><span class="Apple-converted-space">      </span>"What would your walk-up song be if you entered every room like a professional athlete?",</p>
<p class="p1"><span class="Apple-converted-space">      </span>"Which fictional creature or character would have the most interesting anatomy?",</p>
<p class="p1"><span class="Apple-converted-space">      </span>"If you had to communicate using only emojis for a day, which three would you rely on most?",</p>
<p class="p1"><span class="Apple-converted-space">      </span>"If your phone could only keep three apps, which would you choose?",</p>
<p class="p1"><span class="Apple-converted-space">      </span>"What show, movie, or game would you recommend to everyone?",</p>
<p class="p1"><span class="Apple-converted-space">      </span>"If you came with a warning label, what would it say?",</p>
<p class="p1"><span class="Apple-converted-space">      </span>"If you had to be haunted by one completely harmless animal, what would you choose?",</p>
<p class="p1"><span class="Apple-converted-space">      </span>"Which fictional character would make the best roommate, and why?"</p>
<p class="p1"><span class="Apple-converted-space">    </span>];</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">    </span>let currentRotation = 0;</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">    </span>function spinWheel() {</p>
<p class="p1"><span class="Apple-converted-space">      </span>const wheel = document.getElementById("wheel");</p>
<p class="p1"><span class="Apple-converted-space">      </span>const result = document.getElementById("result");</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">      </span>result.textContent = "Spinning...";</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">      </span>const randomIndex = Math.floor(Math.random() * questions.length);</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">      </span>const degreesPerSlice = 360 / questions.length;</p>
<p class="p1"><span class="Apple-converted-space">      </span>const extraSpins = 5 * 360;</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">      </span>const stopAngle = randomIndex * degreesPerSlice;</p>
<p class="p1"><span class="Apple-converted-space">      </span>const finalRotation = extraSpins + (360 - stopAngle);</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">      </span>currentRotation += finalRotation;</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">      </span>wheel.style.transform = `rotate(${currentRotation}deg)`;</p>
<p class="p2"><br></p>
<p class="p1"><span class="Apple-converted-space">      </span>setTimeout(() =&gt; {</p>
<p class="p1"><span class="Apple-converted-space">        </span>result.textContent = questions[randomIndex];</p>
<p class="p1"><span class="Apple-converted-space">      </span>}, 4000);</p>
<p class="p1"><span class="Apple-converted-space">    </span>}</p>
<p class="p1"><span class="Apple-converted-space">  </span>&lt;/script&gt;</p>
<p class="p2"><br></p>
<p class="p1">&lt;/body&gt;</p>
<p class="p1">&lt;/html&gt;</p>
</body>
</html>
