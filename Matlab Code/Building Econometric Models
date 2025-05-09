% Задаю коэффициент наклона из Спецификации 1.1:
b_alu = 0.214089
b_cop = 0.255858
b_gas = 0.065226
b_gasus = 0.210104
b_cop1 = 0.130405
b_cop2 = 0.206061
b_gas1 = -0.006883
b_gas2 = 0.119692

% Алюминий:
% Спецификация 1
indep = comm.oil_ln_diff(2:t)
dep = comm.aluminum_ln_diff(2:t)
k=2
S=[1 0]
advOpt.distrib='Normal'
advOpt.std_method=1
advOpt.constCoeff.covMat{1}(1 ,1)={'e'}
advOpt.constCoeff.covMat{2}(1 ,1)={'e'}
advOpt.constCoeff.p={'e','e';'e','e'}
advOpt.constCoeff.nS_Param{1}={'e'}
advOpt.constCoeff.S_Param{1}={'e', 'e'}
Spec_Out=MS_Regress_Fit (dep, indep, k, S, advOpt)

% Спецификация 2
indep = comm.oil_ln(1:t)
dep = comm.aluminum_ln(1:t)

dep = dep - (indep * b_alu)
n = size(dep, 1)
v = ones(n,1)
indep = v

S=[1 0]
k=2
advOpt.std_method=1
advOpt.constCoeff.covMat{1}(1 ,1)={'e'}
advOpt.constCoeff.covMat{2}(1 ,1)={'e'}
advOpt.constCoeff.p={'e','e';'e','e'}
advOpt.constCoeff.nS_Param{1}={'e'}
advOpt.constCoeff.S_Param{1}={'e', 'e'}
Spec_Out=MS_Regress_Fit (dep, indep, k, S, advOpt)




% Медь:
% Спецификация 1
indep = comm.oil_ln_diff(2:t)
dep = comm.copper_ln_diff(2:t)
k=2
S=[1 0]
advOpt.distrib='Normal'
advOpt.std_method=1
advOpt.constCoeff.covMat{1}(1 ,1)={'e'}
advOpt.constCoeff.covMat{2}(1 ,1)={'e'}
advOpt.constCoeff.p={'e','e';'e','e'}
advOpt.constCoeff.nS_Param{1}={'e'}
advOpt.constCoeff.S_Param{1}={'e', 'e'}
Spec_Out=MS_Regress_Fit (dep, indep, k, S, advOpt)

% Спецификация 2
indep = comm.oil_ln(1:t)
dep = comm.copper_ln(1:t)

dep = dep - (indep * b_cop)
n = size(dep, 1)
v = ones(n,1)
indep = v

S=[1 0]
k=2
advOpt.std_method=1
advOpt.constCoeff.covMat{1}(1 ,1)={'e'}
advOpt.constCoeff.covMat{2}(1 ,1)={'e'}
advOpt.constCoeff.p={'e','e';'e','e'}
advOpt.constCoeff.nS_Param{1}={'e'}
advOpt.constCoeff.S_Param{1}={'e', 'e'}
Spec_Out=MS_Regress_Fit (dep, indep, k, S, advOpt)


% Медь (выборка с 2010 года):
% Спецификация 1
indep = comm.oil_ln_diff(250:t)
dep = comm.copper_ln_diff(250:t)
k=2
S=[1 0]
advOpt.distrib='Normal'
advOpt.std_method=1
advOpt.constCoeff.covMat{1}(1 ,1)={'e'}
advOpt.constCoeff.covMat{2}(1 ,1)={'e'}
advOpt.constCoeff.p={'e','e';'e','e'}
advOpt.constCoeff.nS_Param{1}={'e'}
advOpt.constCoeff.S_Param{1}={'e', 'e'}
Spec_Out=MS_Regress_Fit (dep, indep, k, S, advOpt)

% Спецификация 2
indep = comm.oil_ln(250:t)
dep = comm.copper_ln(250:t)

dep = dep - (indep * b_cop2)
n = size(dep, 1)
v = ones(n,1)
indep = v

S=[1 0]
k=2
advOpt.std_method=1
advOpt.constCoeff.covMat{1}(1 ,1)={'e'}
advOpt.constCoeff.covMat{2}(1 ,1)={'e'}
advOpt.constCoeff.p={'e','e';'e','e'}
advOpt.constCoeff.nS_Param{1}={'e'}
advOpt.constCoeff.S_Param{1}={'e', 'e'}
Spec_Out=MS_Regress_Fit (dep, indep, k, S, advOpt)





% Газ (Европа):
% Спецификация 1
indep = comm.oil_ln_diff(2:t)
dep = comm.gas_ln_diff(2:t)
k=2
S=[1 0]
advOpt.distrib='Normal'
advOpt.std_method=1
advOpt.constCoeff.covMat{1}(1 ,1)={'e'}
advOpt.constCoeff.covMat{2}(1 ,1)={'e'}
advOpt.constCoeff.p={'e','e';'e','e'}
advOpt.constCoeff.nS_Param{1}={'e'}
advOpt.constCoeff.S_Param{1}={'e', 'e'}
Spec_Out=MS_Regress_Fit (dep, indep, k, S, advOpt)

% Спецификация 2
indep = comm.oil_ln(1:t)
dep = comm.gas_ln(1:t)

dep = dep - (indep * b_gas)
n = size(dep, 1)
v = ones(n,1)
indep = v

S=[1 0]
k=2
advOpt.std_method=1
advOpt.constCoeff.covMat{1}(1 ,1)={'e'}
advOpt.constCoeff.covMat{2}(1 ,1)={'e'}
advOpt.constCoeff.p={'e','e';'e','e'}
advOpt.constCoeff.nS_Param{1}={'e'}
advOpt.constCoeff.S_Param{1}={'e', 'e'}
Spec_Out=MS_Regress_Fit (dep, indep, k, S, advOpt)


% Газ (Европа) с 2006 года:
% Спецификация 1
indep = comm.oil_ln_diff(200:t)
dep = comm.gas_ln_diff(200:t)
k=2
S=[1 0]
advOpt.distrib='Normal'
advOpt.std_method=1
advOpt.constCoeff.covMat{1}(1 ,1)={'e'}
advOpt.constCoeff.covMat{2}(1 ,1)={'e'}
advOpt.constCoeff.p={'e','e';'e','e'}
advOpt.constCoeff.nS_Param{1}={'e'}
advOpt.constCoeff.S_Param{1}={'e', 'e'}
Spec_Out=MS_Regress_Fit (dep, indep, k, S, advOpt)

% Спецификация 2
indep = comm.oil_ln(200:t)
dep = comm.gas_ln(200:t)

dep = dep - (indep * b_gas2)
n = size(dep, 1)
v = ones(n,1)
indep = v

S=[1 0]
k=2
advOpt.std_method=1
advOpt.constCoeff.covMat{1}(1 ,1)={'e'}
advOpt.constCoeff.covMat{2}(1 ,1)={'e'}
advOpt.constCoeff.p={'e','e';'e','e'}
advOpt.constCoeff.nS_Param{1}={'e'}
advOpt.constCoeff.S_Param{1}={'e', 'e'}
Spec_Out=MS_Regress_Fit (dep, indep, k, S, advOpt)


% Газ (США):
% Спецификация 1
indep = comm.oil_ln_diff(2:t)
dep = comm.gasus_ln_diff(2:t)
k=2
S=[1 0]
advOpt.distrib='Normal'
advOpt.std_method=1
advOpt.constCoeff.covMat{1}(1 ,1)={'e'}
advOpt.constCoeff.covMat{2}(1 ,1)={'e'}
advOpt.constCoeff.p={'e','e';'e','e'}
advOpt.constCoeff.nS_Param{1}={'e'}
advOpt.constCoeff.S_Param{1}={'e', 'e'}
Spec_Out=MS_Regress_Fit (dep, indep, k, S, advOpt)

% Спецификация 2
indep = comm.oil_ln(1:t)
dep = comm.gasus_ln(1:t)

dep = dep - (indep * b_gasus)
n = size(dep, 1)
v = ones(n,1)
indep = v

S=[1 0]
k=2
advOpt.std_method=1
advOpt.constCoeff.covMat{1}(1 ,1)={'e'}
advOpt.constCoeff.covMat{2}(1 ,1)={'e'}
advOpt.constCoeff.p={'e','e';'e','e'}
advOpt.constCoeff.nS_Param{1}={'e'}
advOpt.constCoeff.S_Param{1}={'e', 'e'}
Spec_Out=MS_Regress_Fit (dep, indep, k, S, advOpt)
