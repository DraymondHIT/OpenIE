# OpenIE
Open Information Extraction

## Example

The following example sentence is from SQuAD 1.1

```
European Union law is a body of treaties and legislation, such as Regulations and Directives, which have direct effect or indirect effect on the laws of European Union member states.
```

## Stanford's OpenIE

[Python wrapper for Stanford OpenIE](https://github.com/philipperemy/Stanford-OpenIE-Python): The unofficial cross-platform Python wrapper for the state-of-art information extraction library from Stanford University.

Result:

```
{'subject': 'European Union law', 'relation': 'is', 'object': 'body'}
{'subject': 'European Union law', 'relation': 'is body of', 'object': 'treaties'}
```

## AllenNLP's OpenIE

A reimplementation of a deep BiLSTM sequence prediction model ([Stanovsky et al., 2018](https://aclanthology.org/N18-1081/))

Result:

```
'[ARG1: European Union law] [V: is] [ARG2: a body of treaties and legislation , such as Regulations and Directives , which have direct effect or indirect effect on the laws of European Union member states] .'
'European Union law is a body of treaties and legislation , such as [ARG0: Regulations and Directives] , [R-ARG0: which] [V: have] [ARG1: direct effect or indirect effect on the laws of European Union member states] .'
```

