![image](https://github.com/DanjaBali/Advanced-java/assets/48566297/5e383014-2997-4db5-8c6c-5b6f0a5491b9)
![image](https://github.com/DanjaBali/Advanced-java/assets/48566297/e3a8af97-5257-47b5-ab26-0f836aec85cd)
![image](https://github.com/DanjaBali/Advanced-java/assets/48566297/bb0dea8d-97cb-488a-b049-5b9d738fd289)
![image](https://github.com/DanjaBali/Advanced-java/assets/48566297/75cf9416-4a01-40bb-a7a4-59a8409a86e7)


Implementation:
The program is implemented mainly with the followingclasses, and methods respectively.

The MainAppOfNGramer class includes following methods and operations: The execute() method is responsible for calling and executing all unigram, twogram, cosineSimilarity and threads methods.

The unigram() method, separate the sentences in single words and we count the occurrence of each word in the text. To do this we have used a for each and while loops. Also, for navigating the list we have used map Iterator.

The bigram() method, separate the word in two pair letters and count the occurrence of each pair. We have removed all white spaces, punctuation, and have standardize letters into lower case. Moreover, with a for each we calculate the distribution frequency of each pair of letters.

The similarityBetweenDocs() method is used to find the similarity between docs. It saves the content of each file and then, reads text and compare the content. After that with getCosineSimilarityWith() which take as parameter languagesfiles it calculates the cosine similarity of file mystery with first language and then with the second language subfolder.

The readFiles() method read files directoryPath, and fileExtensionToRead and enable us to add dynamically as many files as we want.

The NGramRepositoryFromFileImpl class is used to calculate the similarity of languages given in respective text files as we described above. Method to complete this task are run() -contains the code that the thread will execute.

incCount() method, getCosineSimilarityWith() method, getNorm() method, and getCount method. In addition, this class is intended to be executed by a thread that’s why it also implements runnable interface.

The FileContent class saves the content of all files for each languages, with the help of geter and seter methods. The language class help us to read the path of language folders. The NGram class help us make the calculation for Bigram calculation. It implements iterator interface. We have two overridden method here, hasNext() method and Next() method which make possible to return two pair of letters, BiGram length -2 letters. The class FileSimilarity help us to save the similarity between files.

Conclusion:
The natural language processing Java program, successfully preform the task of language classification. And construct two language models in Java, Albanian, English. It also calculates the document distance, otherwise known as cosine similarity of each language model. The program makes use of streams and lambdas in order to concisely process the text data and update the language models via threads. This enables the program to perform language classification effectively and efficiently.
