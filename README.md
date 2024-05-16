import java.io.IOException;
import java.io.PrintWriter;
import javax.servlet.annotation.WebServlet;
import javax.servlet.http.HttpServlet;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;

@WebServlet("/video-editor")
public class VideoEditorServlet extends HttpServlet {
    @Override
    protected void doGet(HttpServletRequest request, HttpServletResponse response) throws IOException {
        response.setContentType("text/html");
        PrintWriter out = response.getWriter();

        // HTML content for the video editing page
        out.println("<!DOCTYPE html>");
        out.println("<html>");
        out.println("<head>");
        out.println("<meta charset=\"UTF-8\">");
        out.println("<meta name=\"viewport\" content=\"width=device-width, initial-scale=1.0\">");
        out.println("<title>Shimpoo Video Editor</title>");
        out.println("<link rel=\"stylesheet\" href=\"styles.css\">");
        out.println("</head>");
        out.println("<body>");
        out.println("<header>");
        out.println("<h1>Shimpoo Video Editor</h1>");
        out.println("</header>");
        out.println("<main>");
        out.println("<p>Welcome to Shimpoo Video Editor. Here you can edit your videos with ease.</p>");
        out.println("</main>");
        out.println("<footer>");
        out.println("<p>&copy; 2024 Shimpoo Video Editor. All rights reserved.</p>");
        out.println("</footer>");
        out.println("</body>");
        out.println("</html>");
    }
}

