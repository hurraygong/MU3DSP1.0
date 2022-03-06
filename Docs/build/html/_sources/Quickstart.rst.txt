Quickstart
----------

Quikly Run scGNN
^^^^^^^^^^^^^^^^
SCpre-seq is a example to run SCpre-seq.




    parser = argparse.ArgumentParser(description='Download PDBfiles from G2s & get features')
    # parser.add_argument('-l', '--variant-site', dest='variant_list', type=str,
    #                     required=True, help='A list of variants, one per line in the format "POS WT MUT", a file')

    parser.add_argument('-w', '--variant-wildtype', dest='variant_wildtype', type=str,
                        required=True, help='wild-type residue, for example residue "A"')
    parser.add_argument('-m', '--variant-mutation', dest='variant_mutation', type=str,
                        required=True, help='mutation residue, for example residue "A"')
    parser.add_argument('-p', '--variant-position', dest='variant_position', type=int,
                        required=True, help='variant position in sequence')

    parser.add_argument('-s', '--sequence',  type=str,
                        required=True, help='A protein primary sequence in a file in the format fasta.')

    # background mutation Features from G2s

    parser.add_argument('--pdbpath',  type=str,default='/storage/htc/joshilab/jghhd/SC/stability_change1/datasets_s1676_seq/PDB/',
                        required=True, help='A path for storage matched PDB structures')
    parser.add_argument('--dssppath', type=str,default='/storage/htc/joshilab/jghhd/SC/stability_change1/datasets_s1676_seq/dssp/',
                        required=True, help='A path for storage dssp output files')
    parser.add_argument('--dsspbin',  type=str,default='mkdssp',
                        required=True, help='Execute bin path for DSSP')
    parser.add_argument('--psiblastbin',  type=str,default='psiblast',
                        required=True, help='Execute bin path for psiblast')
    parser.add_argument('--hhblitsbin',  type=str,default='hhblits',
                        required=True, help='Execute bin path for hhblits')

    parser.add_argument('--psiblastout',  type=str,default='./Sequence/psiout',
                        required=True, help='A path for storage psiblast out files')
    parser.add_argument('--psiblastpssm',  type=str,default='./Sequence/pssmout',
                        required=True, help='A path for storage psiblast pssm files')
    parser.add_argument('--psiblastdb',  type=str,default='/home/gongjianting/tools/PsiblastDB/swissprot',
                        required=True, help='background database for align in psiblast')


    parser.add_argument('--hhblitsdb',  type=str,default='/home/gongjianting/tools/HHsuitDB/UniRef30_2020_06',
                        required=True, help='background database for align in tools hhblits')

    parser.add_argument('--hhblitsout',  type=str,default='./Sequence/hhblitout',
                        required=True, help='A path for storage hhblits hhr files')
    parser.add_argument('--hhblitshhm',  type=str,default='./Sequence/hhmout',
                        required=True, help='A path for storage hhblits hhm files')
    parser.add_argument("-v", "--version", action="version")
    parser.add_argument("-o", "--outfilename",required=True,  type=str,help='Output files name')
