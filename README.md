# DataDenoisingFFT

Data denoising using FFT (Fast Fourier Transform) is a widely-used technique for cleaning noisy signals or data in the frequency domain. By transforming the data from the time domain to the frequency domain, it becomes possible to identify and isolate noise frequencies from the signal's actual components. Once the noisy frequencies are identified, they can be attenuated or removed, leaving behind a cleaner version of the data. This process is especially valuable in various fields such as signal processing, image processing, and audio processing, where accurate and noise-free data is crucial for analysis, interpretation, and decision-making.
This code performs signal processing and noise reduction on a noisy signal. (data denoise.mlx)

1. Signal Generation: 
   - Two sine waves with frequencies of 50Hz and 120Hz are created.
   - A noisy signal is generated by adding random noise to the clean signal.

2. Plotting:
   - The code plots three graphs in separate subplots:
     - The original noisy signal and the clean signal.
     - The filtered signal in the time domain.
     - The power spectrum density (PSD) of the noisy and filtered signals in the frequency domain.

3. FFT (Fast Fourier Transform):
   - The FFT is computed on the noisy signal to transform it into the frequency domain.
   - PSD is calculated by taking the magnitude squared of the FFT, representing the power at each frequency.
   - Frequency values in Hz are generated for the x-axis.

4. Filtering:
   - A filter is applied to the PSD to identify and preserve frequencies with significant power while attenuating others.
   - This filter is based on a threshold (PSD > 100) to distinguish significant frequencies.

5. Inverse FFT (iFFT):
   - The filtered FFT is transformed back to the time domain using the inverse FFT, resulting in the filtered signal.
   
6. Plotting Filtered Results:
   - The code plots the filtered signal in the time domain.
   - It also plots the PSD of both the noisy and filtered signals for comparison.
   
In summary, this code demonstrates the process of noisy signal filtering in both the time and frequency domains. It starts by generating a noisy signal, then applies a filter to retain important signal components while removing noise. The filtered signal is then displayed, along with its frequency domain representation.

__________________________________________________________________________________________________________________________________________________________________________________________
ADMM (Alternating Direction Method of Multipliers):
ADMM is an optimization technique used to solve convex optimization problems with constraints. It decomposes the problem into subproblems and iteratively updates primal and dual variables. In each iteration, it alternates between updating the primal variables while holding the dual variables fixed and updating the dual variables while holding the primal variables fixed. ADMM is particularly useful for problems with separable structure or those that can be decomposed into smaller, more manageable subproblems. It's often employed in optimization scenarios where traditional methods may be less efficient or impractical.

admm.mlx
This code implements the Alternating Direction Method of Multipliers (ADMM) algorithm to solve a simple optimization problem with equality constraints.

