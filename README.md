# MIE250 Project3

Please see the assignment description posted on Quercus for instructions.

## Important Message
The following method/constructor will be tested by auto grader. Changing these method name or parameters will resulted in compilation error. If you are worried about breaking the passivity of your code, please confirm with TA for the original method signiature. 

Vector Class:
public HashMap<String,Double> _hmVar2Value    
public Vector()   
public Vector(String s)   
public String toString()   
public void clear()   
public void set(String var, double val)   
public void setAll(Vector x)   
public double computeL2Norm()    
public Vector sum(Vector y) throws VectorException   
public Vector scalarMult(double scalar)   
   
Term Class:   
public double _coef    
public ArrayList<String>  _vars    
public ArrayList<Integer> _pows    
public Term(double coef)   
public Term(String s) throws PolyException   
public String toString()   
public TreeSet<String> getAllVars()   
public double evaluate(Vector assignments) throws PolyException    
public Term differentiate(String var)    
   
Polynomial Class:   
public ArrayList<Term> _terms     
public Polynomial()   
public Polynomial(String s) throws PolyException   
public String toString()   
public static Polynomial ReadPolynomial(File file) throws PolyException   
public TreeSet<String> getAllVars()   
public double evaluate(Vector assignments) throws Exception   
public Polynomial differentiate(String var)   
   
Minimizer Class:   
public double _eps;			// tolerance
public int    _maxIter;		// maximum number of iterations
public double _stepSize;		// step size alpha
public Vector _x0;	   		// starting point
public Vector _lastx; 		// last point found
public double _lastObjVal;		// last obj fn value found
public double _lastGradNorm;   // last gradient norm found
public long _compTime;			// computation time needed
public int _nIter;				// no. of iterations needed
public Minimizer()    
public double getEps()   
public int getMaxIter()   
public double getStepSize()   
public Vector getX0()    
public double getLastObjVal()   
public double getLastGradNorm()   
public Vector getLastPoint()   
public int getNIter()   
public long getCompTime()   
public void setEps(double e)    
public void setMaxIter(int m)     
public void setStepSize(double s)   
public void setX0(Vector x0)   
public void minimize(Polynomial p) throws Exception    
public void printResults(PrintStream ps)   
public void printParams(PrintStream ps)    
