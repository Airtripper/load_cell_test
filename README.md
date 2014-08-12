load-cell-test
==============

Arduino sketch to calibrate the INA125 chip with attached load cell, and output weight in grammes.

ABOUT

This software takes an analog reading from a load cell circuit attached to the arduino.
Each new analog reading is put into a buffer of many readings where the newest
analog reading replaces the oldest analog reading. All the readings in the buffer
are added together and then divided by the number of readings held in the buffer to
yield an average analog value. The buffer is used as a method of smoothing the analog
readings taken from the arduino analog pin.

The software has two modes of operation where one operation is used for calibration and
testing while the other is used for outputting to a graphing application such as
Processing.

LICENSE

See LICENSE file

TERMS

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
