# ph2_session7
Assignment Phase 2 Session 7 (Reinforcement learning self driving car)

The youtube video link is:

https://youtu.be/verSX8kSGS0

Answers to the assignment questions:

What happens when Temperature is reduced? 


The confidence level was very low... It was shaky, keep changing directions, did not coverge at all for a long time.


What is the effect of reducing gamma?

Car was alway sticking to the corners. Did not converge for a long time.

By reducing gamma, the importance of future states was reduced. The current reward is more important.

Qtarget(s,a) = R(s,a) + gamma*max(Q(s',a'))

TD = Sumof(square(Qtarget - Q))

That means TD is low even without making a right next state decesion if gamma is low. So, the network does not converge.


