.document {
        background: white;
        padding: 40px;
        border-radius: 10px;
        box-shadow: 0 4px 15px rgba(0,0,0,0.1);
    }
    
    h1 {
        text-align: center;
        color: #2c3e50;
        border-bottom: 3px solid #3498db;
        padding-bottom: 15px;
        margin-bottom: 30px;
    }
    
    .situation {
        background: #fff3cd;
        border-left: 5px solid #ffc107;
        padding: 20px;
        margin: 25px 0;
        border-radius: 5px;
    }
    
    .objective {
        background: #d1ecf1;
        border-left: 5px solid #17a2b8;
        padding: 20px;
        margin: 25px 0;
        border-radius: 5px;
        text-align: center;
        font-size: 1.1em;
        font-weight: bold;
    }
    
    .strategy-overview {
        display: grid;
        grid-template-columns: repeat(3, 1fr);
        gap: 20px;
        margin: 30px 0;
    }
    
    .strategy-box {
        background: #f8f9fa;
        border: 2px solid #dee2e6;
        border-radius: 10px;
        padding: 20px;
        text-align: center;
        transition: all 0.3s ease;
    }
    
    .strategy-box:hover {
        border-color: #3498db;
        transform: translateY(-2px);
    }
    
    .strategy-box h3 {
        color: #e74c3c;
        margin-bottom: 15px;
    }
    
    .timeline {
        background: white;
        border: 2px solid #e9ecef;
        border-radius: 10px;
        padding: 25px;
        margin: 30px 0;
    }
    
    .week {
        display: flex;
        align-items: center;
        margin: 20px 0;
        padding: 15px;
        background: #f8f9fa;
        border-radius: 8px;
        border-left: 4px solid #28a745;
    }
    
    .week-number {
        background: #28a745;
        color: white;
        border-radius: 50%;
        width: 40px;
        height: 40px;
        display: flex;
        align-items: center;
        justify-content: center;
        font-weight: bold;
        margin-right: 20px;
        flex-shrink: 0;
    }
    
    .key-points {
        display: grid;
        grid-template-columns: repeat(3, 1fr);
        gap: 20px;
        margin: 30px 0;
    }
    
    .point-box {
        background: #f8f9fa;
        padding: 20px;
        border-radius: 10px;
        border-top: 4px solid #3498db;
    }
    
    .point-box h4 {
        color: #2c3e50;
        margin-bottom: 15px;
    }
    
    .warning {
        background: #f8d7da;
        border-left: 5px solid #dc3545;
        padding: 20px;
        margin: 25px 0;
        border-radius: 5px;
    }
    
    .success {
        background: #d4edda;
        border-left: 5px solid #28a745;
        padding: 20px;
        margin: 25px 0;
        border-radius: 5px;
        text-align: center;
        font-weight: bold;
    }
    
    .flow-chart {
        display: flex;
        justify-content: space-between;
        align-items: center;
        margin: 30px 0;
        position: relative;
    }
    
    .flow-item {
        background: white;
        border: 2px solid #3498db;
        border-radius: 10px;
        padding: 15px;
        width: 28%;
        text-align: center;
        position: relative;
    }
    
    .flow-item::after {
        content: '→';
        position: absolute;
        right: -25px;
        top: 50%;
        transform: translateY(-50%);
        font-size: 20px;
        color: #3498db;
    }
    
    .flow-item:last-child::after {
        display: none;
    }
    
    @media print {
        body { background: white; }
        .document { box-shadow: none; }
    }
    
    @media (max-width: 768px) {
        .strategy-overview, .key-points {
            grid-template-columns: 1fr;
        }
        .flow-chart {
            flex-direction: column;
            gap: 20px;
        }
        .flow-item::after {
            content: '↓';
            right: 50%;
            bottom: -25px;
            top: auto;
            transform: translateX(50%);
        }
    }
</style>
