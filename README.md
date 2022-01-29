# SM-Projekt
 
Działanie układu polega na pracy w dwóch trybach: ogrzewanie lub „chłodzenie”, które są regulowane za pomocą wypełnienia PWM, którym steruje regulator PID. Sygnał w sytuacji grzania przez pin PA3 (pin TIM2) wysyła sygnał cyfrowy o stosownym wypełnieniu na tranzystor 2N2222A, który powoduje nagrzewanie się rezystora 5W. 
Podczas nagrzewania rezystora na płytce Nucleo świeci się czerwona dioda użytkownika (LD3). Temperaturę zadaną możemy nadać zmieniając parametr Temperature_setpoint. Gdy temperatura czujnika przekroczy temperaturę zadaną zapala się niebieska dioda (LD2), natomiast gdy obie temperatury są sobie równe tj. temperatura mierzona osiągnęła idealnie temperaturę zadaną świeci się zielona dioda (LD1).
Program jest zabezpieczony przed awarią czujnika – w takiej sytuacji na wyświetlaczu LCD wyświetla się stosowny komunikat oraz w jednym momencie zapalają się diody: czerwona, zielona, niebieska.
