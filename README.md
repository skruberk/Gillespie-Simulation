This function performs a Gillespie-style stochastic simulation of actin
% filaments assembling from a membrane-localized pool of profilin-actin
% complexes. 
%
% INPUT PARAMETERS 
% Nfil - total number of filaments in proximity to the membrane
% Msite - surface density of profilin-binding sites on the membrane
% kvect - vector of rate constants (currently 9)
% PA - concentration of soluble profilin-actin
% maxT - maximum time for simulation
%
% OUTPUT VALUES
% time -- vector with time values of simulation
% Ptot -- total polymer in the filament network
% mpool -- average fractional occupancy of the membrane pools at ss


% Parameters 
% nM - number of free membrane sitesactin
% PA - concentration of profilin-actin complexes
% nMPA - membrane-bound profilin-
% nMPAF - membrane-bound profilin-actin-filament complex
% nMPF - membrane-bound profilin-filament complex
% nMP - membrane-bound profilin
% nF - number of free filaments 
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
function [time,Ptot,mpool,fpool] = membrane_pool(Nfil,Msite,kvect,PA,maxT)
