[## Hi there 👋

<!--
**Maruf5583/Maruf5583** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
](https://img.shields.io/badge/Email-marufhasanash%2540gmail.com-blue?style=flat&logo=gmail
https://img.shields.io/badge/LinkedIn-Connect-blue?style=flat&logo=linkedin
https://img.shields.io/badge/GitHub-Follow-black?style=flat&logo=github

🚀 About Me
I'm a passionate .NET Developer with expertise in building scalable web applications using ASP.NET Core and related technologies. I love solving complex problems and creating efficient, maintainable code.

💻 Tech Stack & Skills
Programming Languages
https://img.shields.io/badge/C%2523-239120?style=for-the-badge&logo=c-sharp&logoColor=white
https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black
https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white

Web Development
https://img.shields.io/badge/ASP.NET%2520Core-512BD4?style=for-the-badge&logo=dotnet&logoColor=white
https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white
https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white
https://img.shields.io/badge/Bootstrap-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white

Databases
https://img.shields.io/badge/SQL%2520Server-CC2927?style=for-the-badge&logo=microsoft-sql-server&logoColor=white

DevOps & Cloud
https://img.shields.io/badge/Azure%2520DevOps-0078D7?style=for-the-badge&logo=azure-devops&logoColor=white
https://img.shields.io/badge/Azure-0089D6?style=for-the-badge&logo=microsoft-azure&logoColor=white

📊 Skill Levels














🔧 Technical Expertise
ASP.NET Core Development
csharp
// Sample API Controller
[ApiController]
[Route("api/[controller]")]
public class ProductsController : ControllerBase
{
    private readonly IProductService _productService;
    
    public ProductsController(IProductService productService)
    {
        _productService = productService;
    }
    
    [HttpGet]
    public async Task<IActionResult> GetProducts()
    {
        var products = await _productService.GetAllAsync();
        return Ok(products);
    }
    
    [HttpPost]
    public async Task<IActionResult> CreateProduct([FromBody] ProductDto productDto)
    {
        var product = await _productService.CreateAsync(productDto);
        return CreatedAtAction(nameof(GetProduct), new { id = product.Id }, product);
    }
}
Database Operations
sql
-- SQL Server Stored Procedure
CREATE PROCEDURE GetActiveProducts
    @CategoryId INT = NULL
AS
BEGIN
    SELECT 
        p.Id,
        p.Name,
        p.Price,
        c.Name as CategoryName,
        p.CreatedDate
    FROM Products p
    INNER JOIN Categories c ON p.CategoryId = c.Id
    WHERE p.IsActive = 1
    AND (@CategoryId IS NULL OR p.CategoryId = @CategoryId)
    ORDER BY p.CreatedDate DESC
END
Frontend Skills
javascript
// JavaScript with AJAX call to ASP.NET Core API
async function fetchProducts() {
    try {
        const response = await fetch('/api/products');
        const products = await response.json();
        
        products.forEach(product => {
            const card = `
                <div class="col-md-4">
                    <div class="card mb-4">
                        <div class="card-body">
                            <h5 class="card-title">${product.name}</h5>
                            <p class="card-text">$${product.price}</p>
                            <button class="btn btn-primary" onclick="addToCart(${product.id})">
                                Add to Cart
                            </button>
                        </div>
                    </div>
                </div>
            `;
            document.getElementById('product-list').innerHTML += card;
        });
    } catch (error) {
        console.error('Error fetching products:', error);
    }
}
📈 GitHub Stats
https://github-readme-stats.vercel.app/api?username=yourusername&show_icons=true&theme=radical

https://github-readme-stats.vercel.app/api/top-langs/?username=yourusername&layout=compact&theme=radical

🏆 GitHub Trophies
https://github-profile-trophy.vercel.app/?username=yourusername&theme=radical&no-frame=true&row=1&column=6

📫 Let's Connect
Email: marufhasanash@gmail.com

LinkedIn: Your LinkedIn Profile

Portfolio: Your Portfolio Website

📁 Featured Projects
🚀 Project 1: E-commerce Platform
Tech Stack: ASP.NET Core, SQL Server, React, Azure

Built a full-featured e-commerce platform with payment integration

Implemented microservices architecture with Docker containers

Achieved 99.9% uptime on Azure Kubernetes Service

🏥 Project 2: Hospital Management System
Tech Stack: ASP.NET Core MVC, Entity Framework, Bootstrap

Developed comprehensive hospital management system

Implemented role-based authentication and authorization

Optimized database queries reducing load time by 60%

)
