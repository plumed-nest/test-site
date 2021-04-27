**Project ID:** [plumID:20.029]({{ '/' | absolute_url }}eggs/20/029/)  
**Source:** E2F1-DP1_PLUMED-NEST/MULTI_REPLICA/plumed-SAXS_12q.dat  
{% raw %}<pre>
<a href="https://plumed.github.io/doc-master/user-doc/html/_s_a_x_s.html">SAXS</a> ...

	LABEL=saxsCG
	ATOMS=martini
	MARTINI
	NOPBC
	<span style="color:blue">#GPU</span>

	SCALEINT=107.069000

	QVALUE1=0.008900	EXPINT1=103.136000
	QVALUE2=0.026714	EXPINT2=77.162100
	QVALUE3=0.044528	EXPINT3=46.442600
	QVALUE4=0.062343	EXPINT4=27.614400
	QVALUE5=0.080157	EXPINT5=19.054000
	QVALUE6=0.097971	EXPINT6=12.904200
	QVALUE7=0.115785	EXPINT7=7.450970
	QVALUE8=0.133599	EXPINT8=4.302110
	QVALUE9=0.151413	EXPINT9=2.881410
	QVALUE10=0.169227	EXPINT10=1.852090
	QVALUE11=0.187041	EXPINT11=1.200270
	QVALUE12=0.204855	EXPINT12=1.021820

	<span style="color:blue"># METAINFERENCE</span>
	DOSCORE
	SIGMA0=2.0 
	SIGMA_MIN=0.001,0.001,0.001,0.001,0.001,0.001,0.001,0.001,0.001,0.001,0.001,0.001
	SIGMA_MAX=0.769355,4.928531,6.467537,3.017866,1.278125,1.699344,0.613271,0.250122,0.195501,0.129698,0.097217,0.083433
	MC_CHUNKSIZE=1 MC_STEPS=12
	NOISETYPE=MGAUSS
	SCALEDATA SCALE_PRIOR=FLAT SCALE0=1.00 SCALE_MIN=0.7 SCALE_MAX=1.3 DSCALE=0.0002
        SIGMA_MEAN0=2 OPTSIGMAMEAN=SEM AVERAGING=100
	WRITE_STRIDE=1000
... <a href="https://plumed.github.io/doc-master/user-doc/html/_s_a_x_s.html">SAXS</a>

saxsbias: <a href="https://plumed.github.io/doc-master/user-doc/html/_b_i_a_s_v_a_l_u_e.html">BIASVALUE</a> ARG=(saxsCG\.score) STRIDE=6
ens: <a href="https://plumed.github.io/doc-master/user-doc/html/_e_n_s_e_m_b_l_e.html">ENSEMBLE</a> ARG=(saxsCG\.q-.*)
statCG: <a href="https://plumed.github.io/doc-master/user-doc/html/_s_t_a_t_s.html">STATS</a> ARG=(ens\.saxsCG\.q-.*) PARARG=(saxsCG\.exp-.*)

<span style="color:blue"># PRINT</span>
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=(saxsCG\.score),(saxsCG\.scale),(saxsCG\.acceptScale),(saxsCG\.acceptSigma),(saxsCG\.sigma.*) STRIDE=500 FILE=BAYES.SAXS
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=(saxsCG\.q-.*) FILE=SAXSINTCG STRIDE=2500
<a href="https://plumed.github.io/doc-master/user-doc/html/_p_r_i_n_t.html">PRINT</a> ARG=statCG.*,(ens\.saxsCG\.q-.*) FILE=ST.SAXSCG STRIDE=2500
</pre>{% endraw %}
