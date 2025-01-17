---
title: Code Delay

# View.
#   1 = List
#   2 = Compact
#   3 = Card
#   4 = Citation
view: 1

# Optional header image (relative to `static/media/` folder).
header:
  caption: ""
  image: ""
---

<p style="padding-top: 0pt; " class="paragraph_style_3">At the bottom of this page, you can download the Matlab source code described in the manuscript &quot;New method to measure end-to-end delay of Virtual Reality&quot; by Massimiliano Di Luca published in <a href="https://direct.mit.edu/pvar/article/19/6/569/18788/New-Method-to-Measure-End-to-End-Delay-of-Virtual">Presence: Teleoperators &amp; Virtual Environments</a>. The manuscript can be downloaded <a href="../publication/di-luca-2010/">HERE</a>. I recommend reading it, as the software is not self-explanatory. <br /></p>
<p class="paragraph_style_3">The code allows the implementation of the method which uses two photodiodes and two gradients (one real shown on a flat panel display, one virtual). The two photodiodes capture the light produced by the gradient on the flat panel display and by the virtual gradient. The signal is thus proportional to the position along the gradient. By plugging the two photodiodes into the audio card, it is possible to record virtual and physical trajectories without additional materials than a computer. The method allows to perform multiple recordings and vary, for example, the movement frequency in order to determine whether the end-to-end delay of the VR system is constant. Other parameters can also be varied to test if the delay changes (movement direction, amplitude of movement, location). The advantages of this method are the simplicity of the measurement and the similarity of the setups required for measurement and for final utilization of the VR system. In the paper I consider different types of VR system where the arrangement required for the measurement changes accordingly, for example:<br /></p>
<ol>
  <li style="line-height: 33px; padding-left: 40px; text-indent: -20px; " class="full-width">
  With VR system having an HMD display, the recordings require to perform repetitive movements of the HMD with attached a photodiode. Movements are performed in front of the flat-panel display. In the VR scene the second gradient is displayed (which position is fixed with respect to the VR environment). The second photodiode points at the display of the HMD. <br /></p>
  </li>
  <li style="line-height: 33px; padding-left: 40px; text-indent: -20px; " class="full-width">
 With VR system having a fixed screen, the recordings are preformed by moving a tracker (with attached a photodiode) in front of the flat-panel display. A second diode captures the luminance generated by the gradient in the VR scene (which position is updated according to the position of the tracker). <br /></p>
  </li>
</ol>
<p class="paragraph_style_3">The analysis script included in the archive allows the estimate of the frequency of movements and of the delay for each of the recordings. <br /><br /></p>
<p class="paragraph_style_3">Content of the archive: <br /></p>
<ol>
  <li style="line-height: 33px; padding-left: 40px; text-indent: -20px; " class="full-width">
  test_{1/2}_{1/2/3/4}.mat </li>
<p class="paragraph_style_3">                set of example recordings <br /></p>

  <li style="line-height: 33px; padding-left: 40px; text-indent: -20px; " class="full-width">
  test_recording.m </li>
  <p class="paragraph_style_3">                to checks whether the diodes are connected correctly and the audiocard has a stereo line-in input <br /></p>

  <li style="line-height: 33px; padding-left: 40px; text-indent: -20px; " class="full-width">
  signal_recording.m </li>
  <p class="paragraph_style_3">                can be used to record the signals generated by one movement <br /></p>

  <li style="line-height: 33px; padding-left: 40px; text-indent: -20px; " class="full-width">
calculate_delay_gui.m </li>
<p class="paragraph_style_3">                loads a series of recordings and determines the relative delay and largest frequency component<br /></p>

  <li style="line-height: 33px; padding-left: 40px; text-indent: -20px; " class="full-width">
  myfilteronefreq.m <br /></li>

  <li style="line-height: 33px; padding-left: 40px; text-indent: -20px; " class="full-width">
  finddelay.m </li>
  <li style="line-height: 33px; padding-left: 40px; text-indent: -20px; " class="full-width">
  fsplot.m </li>
  <li style="line-height: 33px; padding-left: 40px; text-indent: -20px; " class="full-width">
  findfreq.m  </li>

<p class="paragraph_style_3">                files required by calculate_delay_gui.m <br /><br /></p>

<br />
<br />
<br />

<p class="paragraph_style_3">Copyright (c) 2010, Massimiliano Di Luca <br /></p>
<p class="paragraph_style_3">Permission is hereby granted, free of charge, to any person obtaining a copy of this software, the data files, and associated documentation files (the &quot;Software&quot;), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: <br /></p>
<p class="paragraph_style_3">The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software. <br /></p>
<p class="paragraph_style_3">THE SOFTWARE IS PROVIDED &quot;AS IS&quot;, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE. <br /></p>
<br />
<br />
<p><a class="class1" title="delay_measurement_0_3.zip" href="delay_measurement_0_3.zip">I accept the terms</a></p>
<br />
<br />
<br />
