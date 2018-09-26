
\"z"\ = \ \left\{ h,\overline {h}\right\}

\CW_{hap}=\left\{ H_{1}\right\} \left\{ H_{2}\right\} \ldots \left\{ H_{z}\right\}

\CW_{hap}=\left\{\begin{aligned}\overline {h_{1}}\\ h_{1}\end{aligned}\right\} \left\{\begin{aligned}\overline {h_{2}}\\ h_{2}\end{aligned}\right\} \ldots \left\{\begin{aligned}\overline {h_{z}}\\ h_{z}\end{aligned}\right\}


\The most likely haplotype state 
\H = \left\{ h,\overline {h}\right\} 

\given two consecutive haplotype,

\Block 1:  H_{1} = \left\{ h_{1},\overline {h_{1}}\right\}

\Block 2:  H_{2} = \left\{ h_{2},\overline {h_{2}}\right\}

\can be,

\H=\begin{cases}\left\{ h_{1}h_{2},\overline {h_{1}}\overline {h_{2}}\right\} \\ \left\{ h_{1}\overline {h_{2}},\overline {h_{1}}h_{2}\right\} \end{cases}

\H=\begin{cases}\left\{ h_{1}h_{2},\overline {h_{1}}\overline {h_{2}}\right\} ^{\nearrow parallel-configuration }_{OR}\\ \left\{ h_{1}\overline {h_{2}},\overline {h_{1}}h_{2}\right\} ^{\searrow alternate-configuration}\end{cases}

\Using markov chain transition (from each site in Block 1 to each site in Block 2) we compute likelihood of the each possible configuration:

\h,\overline {h}=\begin{cases}\left( h_{1}h_{2}\right) ,\left( \overline {h_{1}},\overline {h_{2}}\right) ^{\longrightarrow with likelihood (L{_1}) }\\ \left( h_{1}\overline {h_{2}}\right) ,\left( \overline {h_{1}}h_{2}\right) ^{\longrightarrow with likelihood (L{_2}) }\end{cases}

