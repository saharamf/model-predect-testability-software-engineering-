# model-predect-testability-software-engineering-
this program used to predect testability from program matrices in python
import pandas as pd
import sklearn as sk
import matplotlib.pyplot as plt

dt=pd.read_csv('result_evosuite_water_simulatore before refactor1.csv')

dt
dt.isnull().sum()
fet=['ctg_min_time_per_job','search_budget','p_object_pool','ctg_time_per_class','Size','Length','Total_Time','LineCoverage','BranchCoverage','ExceptionCoverage','Explicit_MethodExceptions','Explicit_TypeExceptions','Implicit_MethodExceptions','Explicit_TypeExceptions','WeakMutationScore','OutputCoverage','MethodCoverage','MethodNoExceptionCoverage','CBranchCoverage']
x_fet=dt[fet]
x_fet
y= dt['testability']
y
