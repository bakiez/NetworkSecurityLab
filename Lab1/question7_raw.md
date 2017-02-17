
The beamwidth, i.e., the angle between the two half-power ($-3dB$) points closest to the boresight axis of the antenna, is already shown in figure 5 as purple lines in the lab assignment. Here can be seen that the beamwidth is approximately $\frac{7}{9} * 90^{\circ} = 70^{\circ}$ 

The antenna gives, in boresight, a gain of $8dB$. This extra power is lost because of the free-spaca path loss (FSPL):

$$ FSPL = {\left(\frac{4 \pi d}{\lambda}\right)}^2 = {\left(\frac{4 \pi d f}{c}\right)}^2$$

Here $f$ is the frequency, $d$ the distance, $\lambda$ the wave length and $c$ the speed of light. Now we want to expres the FSPL in $dB$ by doing $FSPL_{dB} = 10*\log_{10}{(FSPL)}$. Now follows:

$$ FSPL_{dB} = 10*\log_{10}{\left({\left(\frac{4 \pi d f}{c}\right)}^2\right)} = 20*\log_{10}{\left({\frac{4 \pi d f}{c}}\right)}$$

$$ FSPL_{dB} = 20*\log_{10}\left(d\right) + 20*\log_{10}\left(f\right) + 20*\log_{10}\left(\frac{4 \pi}{c}\right)$$

$$ FSPL_{dB} = 20*\log_{10}\left(d\right) + 20*\log_{10}\left(f\right) - 147.55$$

Now we re-order the equation and obtain the following:

$$ 20*\log_{10}\left(d\right) = FSPL_{dB} -  20*\log_{10}\left(f\right) + 147.55$$

$$ \log_{10}\left(d\right) = \frac{FSPL_{dB}}{20} - \log_{10}\left(f\right) + 7.3775$$

$$ d = \frac{1}{f} * 10^{ 7.3775 + \frac{FSPL_{dB}}{20}}$$

with $d$ the distance in meters. When we fill in this equation using $f=433 MHz$ and $FSPL_{dB}=8 dB$ we obtain $d = 0.138m$. Note that when the distance is zero one of the following things need to hold: $f = \infty$ or $FSPL = 0$ or $FSPL_{dB} = -\infty$.
