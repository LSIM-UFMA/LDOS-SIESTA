Para gerar LDOS primeiro calculamos as bandas de energia, com as bandas ja construidas medimos os valores do LUMO e do HUMO e adicinamos na flag do arquivo .fdf do siesta:

%block LocalDensityOfStates
 HOMO  LUMO   eV
%endblock LocalDensityOfStates

Depois sera gerado um arquivo .LDOS

Para obtermos mais informações sobre a plotagem da LDOS compilamos o qrquivo ldos_params, em seguida basta executar rho2xsf e alocar as informações assim como se pede.

Para plotagem usando o VESTA basta renomear o arquivo .XSF para .xsf e abrir direto no VESTA.
