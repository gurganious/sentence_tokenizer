# sentence_tokenizer

**Usage**
    
    # Given string s
    sentences = split_into_sentences(s)  # Returns a list of sentences
    
**Example Code**

    for index, token in enumerate(split_into_sentences(s), start = 1):
        print(f'{index}) {token}')

**Tests**

*1. Input*

    s='''It is relevant to point that Case No. 778 - Martin H. v. The Woods, it was mentioned that death
     to one cannot be generalised. However, the High Court while enhancing the same from life to 
    death, in our view,has not assigned adequate and acceptable reasons. In our opinion, it is not a 
    rarest of rare case where extreme penalty of death is called for instead sentence of 
    imprisonment for life as ordered by the trial Court would be appropriate.15) In the light of the 
    above discussion, while maintaining the conviction of the appellant-accused for the offence under Section 302. IPC, 
    award of extreme penalty of death by the High Court is set aside and we restore the sentence of
     life imprisonment as directed by the trial Court.
    '''

*Output*

    1) It is relevant to point that Case No. 778 - Martin H. v. The Woods, it was mentioned that death  to one cannot be generalised.
    2) However, the High Court while enhancing the same from life to  death, in our view,has not assigned adequate and acceptable reasons.
    3) In our opinion, it is not a  rarest of rare case where extreme penalty of death is called for instead sentence of  imprisonment for life as ordered by the trial Court would be appropriate.
    4) 15) In the light of the  above discussion, while maintaining the conviction of the appellant-accused for the offence under Section 302. IPC,  award of extreme penalty of death by the High Court is set aside and we restore the sentence of  life imprisonment as directed by the trial Court.

*2. Input*

    s = '''Mr. or Mrs. or Dr. (not sure of their title) Smith will be here in the morning at eight.He's arriving on flight No. 48213 out of Denver.He'll take the No. 2 bus from the airport.However, he may grab a taxi instead.'''
    
*Output*

    1) Mr. or Mrs. or Dr. (not sure of their title) Smith will be here in the morning at eight.
    2) He's arriving on flight No. 48213 out of Denver.
    3) He'll take the No. 2 bus from the airport.
    4) However, he may grab a taxi instead.

*3. Input*

    s = '''The respondent, in his statement Ex.-73, which is accepted and found to be truthful. The passcode is either No.5, No. 5, No.-5, No.+5.'''

*Output*

    1) The respondent, in his statement Ex.-73, which is accepted and found to be truthful.
    2) The passcode is either No.5, No. 5, No.-5, No.+5.

*4. Input*

    s = '''He went to New York. He is 10 years old.'''

*Output*

    1) He went to New York.
    2) He is 10 years old.

