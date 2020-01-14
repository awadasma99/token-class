# token-class

/**
 * The Token class serves as the building blocks of a Concordance in that
 * each Token holds information specific to each word in a given file.
 *
 * @author Asma Awad
 * @version 1.0
 */
public class Token {
    private String filename;
    private String word;
    private int wordNum;

    Token(String filename, String word, int wordNum) {
        this.filename = filename;
        this.word = word;
        this.wordNum = wordNum;
    }

    /**
     * getWord allows one to access the word associated with a Token
     * @return the word associated with a Token
     */
    public String getWord() {
        return word;
    }

    /**
     * toString provides a String representation of a Token
     * @return a formatted String representing a Token
     */
    public String toString() {
        return (word + " is word " + wordNum + " in the file " + filename);
    }

}
