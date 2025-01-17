# The Kalman Filter: A Mathematical Overview

## Introduction

The Kalman Filter is an iterative mathematical process that estimates the state of a linear dynamic system from a series of noisy measurements. It is widely used in the fields of signal processing, econometrics, and control systems for its robustness and efficiency in handling uncertainty and noise.

## Mathematical Formulation

The Kalman Filter operates in a two-step process: prediction and update. Here, we detail each step involved in its computation.

## State Space Representation

Consider a system whose state at time $t$  is represented by the vector  $x_t$ , which evolves according to the equation:

$$
 x_t = F_t x_{t-1} + B_t u_t + w_t 
$$
 
where:
- $F_t$  is the state transition model which is applied to the previous state  $x_{t-1}$ 
- $B_t$  is the control-input model which is applied to the control vector  $u_t$ 
- $w_t$  is the process noise which is assumed to be drawn from a normal distribution with mean zero and covariance matrix  $Q_t$

The measurement  $z_t$ , which is an observation at time  $t$ , is given by:

$$
 z_t = H_t x_t + v_t 
$$

where:
- $H_t$  is the observation model which maps the true state space into the observed space
- $v_t$  is the observation noise which is assumed to be drawn from a normal distribution with mean zero and covariance matrix  $R_t$ 

## Prediction Phase

The prediction phase projects forward the current state estimate to obtain an a priori estimate for the next time step:

$$
 \hat{x}{t|t-1} = F_t \hat{x}{t-1|t-1} + B_t u_t 
 P_{t|t-1} = F_t P_{t-1|t-1} F_t^T + Q_t 
$$

where:
- p $\hat{x}_{t|t-1}$  is the predicted state estimate
- p $P_{t|t-1}$  is the predicted error covariance.

## Update Phase

The update phase adjusts the projected estimate by an actual measurement at that time:

$$
 K_t = P_{t|t-1} H_t^T (H_t P_{t|t-1} H_t^T + R_t)^{-1} 
$$
$$
 \hat{x}{t|t} = \hat{x}{t|t-1} + K_t (z_t - H_t \hat{x}{t|t-1}) 
$$
$$
 P{t|t} = (I - K_t H_t) P_{t|t-1} 
$$

where:
- $K_t$  is the Kalman Gain,
- $\hat{x}_{t|t}$  is the updated state estimate,
- $P_{t|t}$  is the updated error covariance.

## Advantages of Kalman Filtering 
- Robustness: Effectively handles noisy data.
- Flexibility: Can be adapted to non-linear models via extensions such as the Extended Kalman Filter or Unscented Kalman Filter.
- Real-time: Operates in a recursive manner which makes it suitable for real-time problems.

## Project Scope

This project applies the Kalman Filter to financial datasets, specifically:
- Estimating hidden financial states such as valuations from noisy observable data like stock prices.
- Analyzing relationships between different financial instruments through state estimations.

## Conclusion

The Kalman Filter provides a sophisticated framework for understanding and predicting dynamic systems in finance. This project seeks to harness this capability to offer deeper insights into financial data, contributing to more informed decision-making processes in financial analysis and trading strategies.
