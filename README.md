# Django-AI-Project
Django research in university
<br>
<br>
<br>
<br>
<br>

# Introduce 
<hr>


<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport"
          content="width=device-width, user-scalable=no, initial-scale=1.0, maximum-scale=1.0, minimum-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <!-- BootStrap CSS -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-KK94CHFLLe+nY2dmCWGMq91rCGa5gtU4mk92HdvYe+M/SXH301p5ILy+dN9+nJOZ" crossorigin="anonymous">
</head>
<body>
  <div class="container my-3">
    <div class="accordion" id="accordionExample">
        <div class="accordion-item">
          <h2 class="accordion-header">
            <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseThree" aria-expanded="false" aria-controls="collapseThree">
              #1. Data analyze & Visualization
            </button>
          </h2>
            <br>
          <div id="collapseTwo" class="accordion-collapse collapse" data-bs-parent="#accordionExample">
            <div class="accordion-body">
              <strong>Visualization of sound source data using javascript module</strong>
                <p>
              </p>
                  <img width="1679" alt="image" src="https://github.com/dalabdgw/Piano_Education_Application/assets/112680039/eca95c2a-2ed8-4d2e-b4fd-e7e1dee4a977">
                <img width="1130" alt="image" src="https://github.com/dalabdgw/Piano_Education_Application/assets/112680039/298608b1-bb38-4675-bee3-76ae9ca77e0b">
                <img width="1152" alt="image" src="https://github.com/dalabdgw/Piano_Education_Application/assets/112680039/bec4cf5f-602d-4bbd-b056-f557efee28ed">
            </div>
            <div>
                <br>
                <br>
                <hr>
                <p><strong><code>alphaBars</code></strong> - When set to true each bar's amplitude affects its opacity, i.e., higher bars are rendered more opaque while shorter bars are more transparent. 
                    This is similar to the lumiBars effect, but bars' amplitudes are preserved and it also works on discrete mode and radial spectrum.
                    For effect priority when combined with other settings, see isAlphaBars.
                    Defaults to false.</p>
                <br>
                <br>
                <p><strong><code>ansiBands</code></strong> - When set to true, ANSI/IEC preferred frequencies are used to generate the bands for octave bands modes (see mode). The preferred base-10 scale is used to compute the center and bandedge frequencies, as specified in the ANSI S1.11-2004 standard. When false, bands are based on the equal-tempered scale, so that in 1/12 octave bands the center of each band is perfectly tuned to a musical note.</p>
                 <br>
                <br>
                <p><strong><code>ledBars</code></strong> - True to activate the LED bars effect for frequency bands modes (see mode). This effect can be customized via setLedParams() method. For effect priority when combined with other settings, see isLedBars. See also trueLeds. Defaults to false.</p>
                 <br>
                <br>
                <p><strong><code>lumiBars</code></strong> - This is only effective for frequency bands modes (see mode). When set to true all analyzer bars will be displayed at full height with varying luminance (opacity, actually) instead. lumiBars takes precedence over alphaBars and outlineBars, except on radial spectrum. For effect priority when combined with other settings, see isLumiBars. Defaults to false.</p>
                <br>
                <br>
                <p><strong><code>noteLabels</code></strong> - When set to true displays musical note labels instead of frequency values, in the x axis (when showScaleX is also set to true). For best visualization in octave bands modes, make sure frequencyScale is set to 'log' and ansiBands is set to false, so bands are tuned to the equal temperament musical scale. Defaults to false.</p>
                <br>
                <br>
                <p><strong><code>outlineBars</code></strong> - When true and mode is set to one of the bands modes, analyzer bars are rendered outlined, with customizable fillAlpha and lineWidth. For effect priority when combined with other settings, see isOutlineBars. Defaults to false.</p>
                <br>
                <br>
                <p><strong><code>loRes</code></strong> - True for low resolution mode. Defaults to false. Low resolution mode halves the effective pixel ratio, resulting in four times less pixels to render. This may improve performance significantly, especially in 4K+ monitors. If you want to allow users to interactively toggle low resolution mode, you may need to set a fixed size for the canvas via css.
                    <br>
                    <br>like so:<br>

canvas {
display: block;
width: 100%;
}
                    <br>
                    <br>
                    This will prevent the canvas size from changing, when switching the low resolution mode on and off.
                </p>
                <br>
                <br>
                <p><strong><code>splitGradient</code></strong> - When set to true and channelLayout is dual-vertical, the gradient will be split between channels. When false, both channels will use the full gradient. The effect is illustrated below, using the 'classic' gradient.</p>
                <br>
                <br>
                <p><strong><code>showBgColor</code></strong> - Determines whether the canvas background should be painted. If true, the background color defined by the current gradient will be used. Opacity can be adjusted via bgAlpha property, when overlay is true. If false, the canvas background will be painted black when overlay is false, or transparent when overlay is true. See also registerGradient(). Defaults to true.</p>
                <br>
                <br>
                <p><strong><code>showFPS</code></strong> - True to display the current frame rate. Defaults to false.</p>
                <br>
                <br>
                <p><strong><code>showPeaks</code></strong> - True to show amplitude peaks. Defaults to true.</p>
                <br>
                <br>
                <p><strong><code>showScaleX</code></strong> - True to display scale labels on the x axis. See also noteLabels. Defaults to true.</p>
                <br>
                <br>
                <p><strong><code>showScaleY</code></strong> - True to display the level/amplitude scale on the y axis. This option has no effect when radial or lumiBars are set to true. When linearAmplitude is set to false (default), labels are shown in decibels (dB), otherwise, values represent a percentage (0-100%) of the maximum amplitude. See also minDecibels and maxDecibels. Defaults to false.</p>
            </div>
            <div>
            <br>
            <br>
                <hr>
                <h4> Time - Amplitude chart </h4>
                <p>The x-axis represents time and the y-axis represents amplitude. The amplitude change corresponding to the time of the sound data is visualized and shown. You can also move the scrollbar below to cut and view only the information on the desired section.</p>
                <br>
                <br>
                <h4> Code - Pitch chart </h4>
                <p>The x-axis represents the scale, and the y-axis represents the pitch of the scale. It is a chart that analyzes and shows the pitch of scales appearing in sound data. The analysis information can be viewed by enlarging the desired part through drag, and the analysis chart can be stored as an image. For example, the pitch of "D₄" is about 400, while that of "G₅" is close to 800.</p>
                <hr>
            </div>
        </div>
        </div>
            <br>
            <br>
            <br>
            <br>
            <br>
        <div class="accordion-item">
          <h2 class="accordion-header">
            <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseTwo" aria-expanded="false" aria-controls="collapseTwo">
              #2. AI Tech
            </button>
          </h2>
          <div id="collapseTwo" class="accordion-collapse collapse" data-bs-parent="#accordionExample">
            <div class="accordion-body">
              <strong><code>To be developed</code></strong>
            </div>
          </div>
            <br>
            <br>
            <br>
            <br>
            <br>
        <div class="accordion-item">
          <h2 class="accordion-header">
            <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseThree" aria-expanded="false" aria-controls="collapseThree">
              #3. Django & AI research website
            </button>
          </h2>
          <div id="collapseThree" class="accordion-collapse collapse" data-bs-parent="#accordionExample">
            <div class="accordion-body">
                <strong>Development of django and ai tech synthetic services</strong>
                <p>
                    <h3>- Environment -</h3><br>
                    Python 3.8    <br>
                    Django framework    <br>
                    Echart    <br>
                    Bootstrap 5.1.3    <br>
                    HTML/CSS/JS vanilla    <br>
                    <br />
                    <h3>- Module -</h3> <br>
                    Librosa    <br>
                    PIL    <br>
                    Pyscript    <br>
                    Scipy    <br>
                    Numpy    <br>
                    Matplotlib    <br>
                    <br>
                </p>
          </div>
        </div>
      </div>
  </div>
</body>
