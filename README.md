# Os-project-
Deadlock detection 
# ====================== Module 3: Main ======================
if __name__ == "__main__":
    root = Tk()
    app = ResourceAllocationGraphSimulator(root)
    root.mainloop()
    def analyze_graph(self):
        """
        Analyzes the graph for deadlocks and visualizes it.
        """
        if not self.graph.edges:
            messagebox.showerror("Error", "No edges added to the graph.")
            return
             # Draw the graph
        GraphOperations.draw_graph(self.graph)
         Detect deadlock
        deadlock, cycle = GraphOperations.detect_deadlock(self.graph)
        if deadlock:
            messagebox.showwarning("Deadlock Detected", f"Deadlock found in cycle: {cycle}")
            else:
            messagebox.showinfo("No Deadlock", "No deadlock detected.")

          
        
