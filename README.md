# Attention based on Information Maximization

```
       AAAA        IIIIIIIIIIII     MM        MM
     AAA  AAA      IIIIIIIIIIII     MMM      MMM
   AAA      AAA        IIII         MMMM    MMMM
   AAA      AAA        IIII         MMMMMMMMMMMM
   AAAAAAAAAAAA        IIII         MMM  MM  MMM
   AAAAAAAAAAAA        IIII         MMM      MMM
   AAA      AAA        IIII         MMM      MMM
   AAA      AAA    IIIIIIIIIIII     MMM      MMM
   AAA      AAA    IIIIIIIIIIII     MMM      MMM

    ATTENTION  based on INFORMATION MAXIMIZATION
```

# Author
Neil D. B. Bruce

Centre of Vision Research and
Department of Computer Science and Engineering
York University
Current contact: Neil.Bruce@sophia.inria.fr
Last update, April 2009

# References

1. Bruce, N.D.B., Tsotsos, J.K., Saliency,
 Attention, and Visual Search: An Information Theoretic
 Approach, Journal of Vision 9:3, pp.1-24, 2009,
 http://journalofvision.org/9/3/5/, doi:10.1167/9.3.5.

2. Bruce, N.D.B., Tsotsos, J.K., Saliency based on
 Information Maximization. Advances in Neural
 Information Processing Systems, 18.

3. Bruce, N. Features that draw visual attention: An
 information theoretic perspective. Neurocomputing,
 v. 65-66, pp. 125-133, May 2005.

4. Bruce, N.D.B., Tsotsos, J.K., Spatiotemporal Saliency:
Towards a Hierarchical Representation of Visual
Saliency, 5th Int. Workshop on Attention in Cognitive
Systems, Santorini Greece, May 12, 2008.

5. Bruce, N.D.B., Tsotsos, J.K., An Information Theoretic
Model of Saliency and Visual Search, L. Paletta
and E. Rome (Eds.): WAPCV 2007, LNAI 4840,
pp. 171–183, 2007.

6. Bruce, N.D.B., Image analysis through local information
measures. In Proceedings of the 17th International
Conference on Pattern Recognition, Cambridge, UK, 2004.

# Usage

There is a single required argument which is the image name, however there are additional arguments which may slightly alter the behavior since many of these require different sub-arguments they require editing the parameters in the code itself, that said, there are a few parameters that are directly accessible from the command line:

## Basic example

```Matlab
out = AIM(imagename);

% With optional arguments:
% resizesize - A scaling factor (% original image size)
% convolve - convolve the output with a gaussian?
% basisname - the feature set e.g. 21jade950, 31infomax975
%   The latter 3 digits correspond to the variance retained
%   in PCA which precedes the ICA method named.
% output - show some visualization. This may require
%   changing some parameters appearing in the code
%   depending on the desired "look".

% out = AIM(imagename,resizesize,convolve,basisname,output);
out2 = AIM('23.jpg',0.5,1,'21jade950.mat',1);
```

Additional options are specified in the parameters that follow including the ability to modify parameters of the computation not available on the command line.

# COPYRIGHT NOTICE

THIS SOFTWARE IS THE PROPERTY OF ITS AUTHOR
NEIL D. B. BRUCE. THE AUTHOR GRANTS PERMISSION TO
DISTRIBUTE THE SOFTWARE IN ITS ORIGINAL FORM WITHOUT
MODIFICATION. UNDER SUCH CIRCUMSTANCES THE COPYRIGHT
NOTICE AND FUNCTIONALITY OF THE SOFTWARE MUST REMAIN
ENTIRELY INTACT INCLUDING ALL SYNTACTIC AND
SEMANTIC ELEMENTS OF ITS FUNCTION. THE AUTHOR GRANTS
A NON-EXLUSIVE LICENSE TO INDIVIDUALS WISHING TO USE
THE SOFTWARE FOR NON-PROFIT RESEARCH PURPOSES. THOSE
WISHING TO EMPLOY THE SOFTWARE FOR COMMERCIAL OR PROFIT
SEEKING ENDEAVORS SHOULD CONTACT THE AUTHOR TO DISCUSS
LICENSING.

DERIVATIVE WORKS ARE ALLOWED BY INDIVIDUALS FOR
NON-PROFIT RESEARCH PURPOSES. SUCH DERIVATIVE WORKS
MAY NOT BE DISTRIBUTED WITHOUT WRITTEN CONSENT OF THE
AUTHOR. ANY WORKS THAT USE THE ABOVE SOFTWARE IN WHOLE
OR PART FOR A COMMERCIAL APPLICATION MUST OBTAIN A
VALID LICENSE FROM THE AUTHOR.

THIS SOFTWARE IS PROVIDED BY THE AUTHOR "AS IS"   AND
ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY
AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED.
IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY DIRECT,
INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF
USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)
HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER
IN CONTRACT, STRICT LIABILITY, OR TORT
(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY
OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF
THE POSSIBILITY OF SUCH DAMAGE.