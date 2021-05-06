
# Symbol affixes






# Rumanian morphological analyser


# Sublexica for Noun
































# Sublexica for Verb














| --- 

| --- 






| --- 











































































# Sublexica for Adjective




# Rumenian morphological analyser

 # Definitions for Multichar_Symbols

## Analysis symbols
The morphological analyses of wordforms for the Romanian
language are presented in this system in terms of the following symbols.
(It is highly suggested to follow existing standards when adding new tags).
## Tags for POS

 * +N +V +A : Open POS's
 * +Adv +CC +CS +Interj +Pron +Num : Open POS's

 * +Symbol = independent symbols in the text stream, like £, €, ©

## Verbal MSP

 * +Prs +Prt +Prf
 * +Ind +Imp +Conj +Opt +Sbj
 * +Sg1 +Sg2 +Sg3 +Pl1 +Pl2 +Pl3
 * +Inf


## Nominal MSP

 * +Msc +Fem +Neu
 * +Sg +Pl +Def +ef
 * +Nom +Gen +Voc
 * +Dem +Pers
 * +Adc +Ord
 * +Indef +Def

 * %>
 * %^AA %^EA %^OA

## Flag diacritics
We have manually optimised the structure of our lexicon using following
flag diacritics to restrict morhpological combinatorics - only allow compounds
with verbs if the verb is further derived into a noun again:
 |  @P.NeedNoun.ON@ | (Dis)allow compounds with verbs unless nominalised
 |  @D.NeedNoun.ON@ | (Dis)allow compounds with verbs unless nominalised
 |  @C.NeedNoun@ | (Dis)allow compounds with verbs unless nominalised

For languages that allow compounding, the following flag diacritics are needed
to control position-based compounding restrictions for nominals. Their use is
handled automatically if combined with +CmpN/xxx tags. If not used, they will
do no harm.
 |  @P.CmpFrst.FALSE@ | Require that words tagged as such only appear first
 |  @D.CmpPref.TRUE@ | Block such words from entering ENDLEX
 |  @P.CmpPref.FALSE@ | Block these words from making further compounds
 |  @D.CmpLast.TRUE@ | Block such words from entering R
 |  @D.CmpNone.TRUE@ | Combines with the next tag to prohibit compounding
 |  @U.CmpNone.FALSE@ | Combines with the prev tag to prohibit compounding
 |  @P.CmpOnly.TRUE@ | Sets a flag to indicate that the word has passed R
 |  @D.CmpOnly.FALSE@ | Disallow words coming directly from root.

Use the following flag diacritics to control downcasing of derived proper
nouns (e.g. Finnish Pariisi -> pariisilainen). See e.g. North Sámi for how to use
these flags. There exists a ready-made regex that will do the actual down-casing
given the proper use of these flags.
 |  @U.Cap.Obl@ | Allowing downcasing of derived names: deatnulasj.
 |  @U.Cap.Opt@ | Allowing downcasing of derived names: deatnulasj.




We describe here how abbreviations are in Romanian are read out, e.g.
for text-to-speech systems.

For example:

 * s.:syntynyt # ;  
 * os.:omaa% sukua # ;  
 * v.:vuosi # ;  
 * v.:vuonna # ;  
 * esim.:esimerkki # ; 
 * esim.:esimerkiksi # ; 


















































% komma% :,      Root ;
% tjuohkkis% :%. Root ;
% kolon% :%:     Root ;
% sárggis% :%-   Root ; 
% násti% :%*     Root ; 

